# creating universal javascript applications
## blurb that says "it'll get techie"
## What happens when you pull the JavaScript rug out from under the feet of your client side app?  If your answer is "White Screen of Death" then come along and see how to create accessible JavaScript apps that run on both client and server side.

# Slide 1

(universe pic)

> We'll be telling you about the pros and cons of universal applications
> and inspire you to create your own

> This will get techie...

# Slide 2

A brief history of client side applications

> Back in the day, the server was king.  We'd render our pages on the server side, chuck it over to the client, and then use things like JavaScript to add little bits of interaction on top.  Things like autocomplete.
> After Web 2.0, users increasingly expected richer, more engaging experiences.  So, more and more JS started being included on the client side to enable this.
> Eventually, in the last few years, developers have been relying on the server less and less, in fact in many cases almost entirely doing away with the server altogether.


# Slide 3

Why is this a problem?

> What happens when you pull the JavaScript rug out from under the feet of your client side app?

 - You're losing money
 > 1% ish no js https://gds.blog.gov.uk/2013/10/21/how-many-people-are-missing-out-on-javascript-enhancement/

 - You're losing money
 > churn for bad load times according to Google research: https://www.doubleclickbygoogle.com/articles/mobile-speed-matters/

 - You're losing money
 > SEO visibility

 - Think of the people!
 > accessibility

# Slide 4

"When an escalator fails, it becomes stairs."
>https://jakearchibald.com/2013/progressive-enhancement-still-important/

> Web app equivalent of an escalator:
>https://help.nowtv.com/

> Web app equivalent of a lift:
> This is what happens when you try to load instagram without JavaScript support.
> https://www.instagram.com/?hl=en


# Slide 5

Disclaimer: it depends on what you're building.


# Slide 6

> Other solutions:
> crappy connection/load times for second visit: service workers (load for first time, need js, but once offline still works.)
> google better at SEO for client side apps (but bing aren't)
> initial load time: other performance optimisations e.g. caching
> BUT none of these has quite as big an impact as reducing the initial download size.
> noscript - tag that runs if no js




>- blogs, sales journeys, etc...
> quick wins:
> push state transitions
- no page refresh, less requests, better performance
- show my blog

# Slide 3

    Write it once; use it everywhere.

> A universal application runs the same piece of code on both server and client side (when we say client we mean browser/mobile).
>



# Slide 3

Why make them?
image of someone asking WHY??!

> see below


# Slide 5

performance
(image of racing)

# Slide 6

Demo




- what
  -
- why
  - accessibility
    - not everyone has JS
    - reasons for not having JS
    - should notify user if they need to turn on JS
    - better if simpler UX (i.e. loading spinner guff) so consistent landing page
  - performance
    - processing before render
    - html down the wire
  - SEO
  - encourages good architecture
    - remove dependencies on DOM
    - find good solutions with inverted dependencies
  - progressive enhancement
  - code sharing
  - both back-end and front end developers
  - 1 repo for client app and api
- when
  - app doesn't need much special JS magic
    - blog / static website
  - fallback to not JS
  - performance critical
    - expected bad connections
- which
  - react
  - meteor/apollo
  - angular2-universal
  - vue
  - etc…
  - Node
  - Other languages + plugins
- how (react)
  - SPA built with components
  - render them into a string (markup)
  - put the app-markup in your HTML page
    - put it inside a known container tag
  - done
  - adding the SPA features
    - make an app.js file
    - use the SPA built with components
    - render it with react onto the same container tag
      - this will see the existing markup is the same and avoid unnecessary work
      - adds event listeners to make the SPA work
- where
  - my blog!
  - boilerplates
    - so many!
    - breko-hub
  - libraries
    - este
    - mean
    - next.js
    - electrode
    - and more
  - awesome-redux
    - overwhelmingly large list of options
