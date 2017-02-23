# creating universal javascript applications
## blurb that says "it'll get techie"
## What happens when you pull the JavaScript rug out from under the feet of your client side app?  If your answer is "White Screen of Death" then come along and see how to create accessible JavaScript apps that run on both client and server side.

# Slide 1

(universe pic)

> We'll be telling you about the pros and cons of universal applications
> and inspire you to create your own

> This will get techie...

# Slide 2

What is a Universal App?

> Single page applications are popular such as Gmail, Google Maps, NowTV Watch and Netflix
> Often these will start with an empty screen that populates on the customers browser

> things that wouldn't be possible without SPAS
  - navigating without a page refresh
  - drag and drop
  - analytics
  - @things in facebook

> This is what an SPA is, an application that runs on the browser
> Making a SPA universal is the process of making it share code with the server to improve performance, accessibility and SEO.

# Slide 3

Why make them?
image of someone asking WHY??!

> see below

# Slide 4

Accessibility
- bullet points

> show some page that has no JS support
> https://www.instagram.com/?hl=en
> talk about solutions
  - show something?!!?!?
> 1% of customers = ££££££
> page that works fine:
  > https://www.google.co.uk
  - blogs, sales journeys, etc...
> quick wins:
  - noscript
> push state transitions
  - no page refres, less requests, better performance
  - show my blog

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
