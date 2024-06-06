

# Web framework for UX developers
Nue is a rapid application development environment for UX developers and other design-minded front-end engineers. It changes the way you think about web development: what used to take a React specialist and thousands of lines of TypeScript is now taken care of with just a few hundred lines of modern CSS.


## Global design system
Nue's secret lies in a thing called _global design system_. It provides web designers, developers, and content creators a common way to structure user interfaces:

! Mega Explainer Image
    Global design system: Layout system, Styling framework, Reactivity, Optimizations
    UX development: standard web stack, 90% CSS

Nue frees you from implementing page layouts and basic UI elements over and over again and uses one system for all your new projects. Your work essentially narrows down to customizing the look and feel through CSS and optionally spice it up with a little bit of JavaScript.


[quote from="Brad Frost" cite="//bradfrost.com/blog/post/a-global-design-system/"]
  Global Design System improves the quality and accessibility of the world’s web experiences, saves the world’s web designers and developers millions of hours, and makes better use of our collective human potential.

Think Nue as a modern-day [CSS Zen Graden](//csszengarden.com/) — a demonstration of what can be accomplished through CSS. Nue just takes it a couple of steps further and expands the idea to a full-blown web development environment.



## For UX developers
Nue is ideal for UX developers who focus on design, accessibility, and the [front of the frontend[brad]. They are fluent with the standard web stack: HTML, CSS, and the basics of JavaScript.


### Less code, mostly CSS
What used to be thousands of lines of TypeScript is narrowed down to just a few hundred lines of CSS. To give you a rough idea, here is the front page source code for both Tailwind and Nue:


[.stack]
  [image.bordered]
    small: /img/react-page.png
    large: /img/react-page-big.png
    caption: Tailwind front page made with mixed concerns
    width: 500
    href: //github.com/tailwindlabs/tailwindcss.com/blob/master/src/pages/index.js

  ---
  [image.bordered]
    small: /img/nue-page.png
    large: /img/nue-page-big.png
    caption: Nue front page with separated content
    width: 500
    href: //github.com/tipiirai/nue/blob/master/new-www/index.md?plain=1


Nue requires significantly less code to build the same thing. For example, this documentation area is made up of ~250 lines of CSS and ~50 lines of optional JavaScript. Contrast this to any React-based documentation generator and you are faced with hundreds of components where the application code is mixed with all the frontend stuff:

[image.gridpaper]
  small: /img/react-vs-ux-dev.png
  large: /img/react-vs-ux-dev-big.png


### Less is More
Today, the amount of JS and CSS on the resulting website can easily get out of hand. The issue is rooted in locally styled components, which are surprisingly large. For example, the combined weight of all CSS on this page is only 7kb, which is smaller than a single [Tailwind button component](/)!

With Nue, you are taking a more [minimalistic approach](practices) to build user-friendly and easily maintainable products that stand the test of time.




### Work closer to standards
[image.floating]
  src: /img/ux-stack.png
  width: 300

Nue embraces the [separation of concerns][soc] principle to isolate your code into clearly distinct layers: content, layout, styling, and reactivity. This increases the clarity of your code and allows you to build websites with vanilla CSS and JavaSript.

The code you are writing now is something that all developers from whatever background can understand for years to come. Because trends come and go, but standards are forever.



### Shift in focus
Instead of learning all the advanced TypeScript concepts and framework-specific idioms, the development focus shifts to building great design and user experience. It's a [whole different mindset][divide]

[table head="| Engineers / React developers | Designers / UX developers"]
  - Focus on | Programming | Design and UX
  - Key technologies | React + Tailwind | Web Standards
  - Primary language | TypeScript | CSS
  - Building blocks | Custom components | Global Design System
  - Key strategy | Tight coupling | Separation of concerns
  - Styling method |  Local styling | External styling
  - Highly valued | Type Safety | Minimalism


In short: UX developers approach product solving from the customer side:

[image.gridpaper]
  small: /img/ux-development.png
  large: /img/ux-development-big.png

You may have the coolest technology choices in the world, with the sickest visual tricks possible, but if the UX fails, everything fails. Or as [Steve Jobs says](//youtu.be/dI93BvrBxQ0?si=Ub2Q_S_E7uKVilVL&t=104):

[quote.floating from="Steve Jobs"]
  You've got to start with the customer experience and work backwards for the technology



## Superior web experiences


### More consistent design and UX
With Nue, you don't need one system for documentation, another for blogging, and yet another for your single-page application. Instead, you have a centrally controlled design system, effectively spread across all areas of your website. This builds a more consistent user experience.

! IMAGE
  Design system -->
    Marketing pages
    Documentation area
    Blogging area
    Product (Single-page app)
    (view transitions)



### Universal view transitions
Nue supports [View Transition API](https://developer.chrome.com/docs/web-platform/view-transitions/) when navigating your website. This lets you use the standard `::view-transition` CSS pseudo-element to fine-tune the animation between page switches. This comes out of the box without any custom custom wiring to your links. Again, you get to learn how the web standard works.

In the future version of Nue, the transitions are supported in single-page applications as well, after which you can seamlessly transition between multi-page- and single-page applications.



### Faster landing pages
Nue-powered sites can offer the same performance levels as text-only websites like [motherfuckingwebsite.com](//motherfuckingwebsite.com/), but without compromising on design. That is: you can get the fastest possible page loads with the design and user experience levels of Stripe or Linear.

Nue [optimizes](performance-optimization) your landing pages to a single, compact HTTP request that has everything to render the full experience:

[image.gridpaper]
  small: /img/first-paint.png
  large: /img/first-paint-big.png


This is pretty much the opposite of what the other frameworks like *Next.js* and *Vite* are doing. They put all their optimization efforts into Rust-based tooling that deals with hundreds, sometimes even thousands of JavaScript files. This may work for single-page applications but is not ideal for content-heavy websites. No amount of JS bundling can beat a single HTTP request that has everything to render the page.




## Faster, happier teams
When the core parts of your web stack are neatly separated your team members can focus on areas they are natively good at.


### Content people
*Marketers, copywriters* and *technical writers* can focus on content in isolation without constant troubling of the developers. All your pages, from rich landing pages to simple blog entries are editable by non-technical people. Here's the difference between Next.js and Nue and how the front page is authored:

[.stack]
  [image.bordered]
    small: /img/mixed-content.png
    large: /img/mixed-content-big.png
    caption: "Next.js: content is found inside JavaScript code
    href: //github.com/tailwindlabs/tailwindcss.com/blob/master/src/pages/index.js#L151

  ---
  [image.bordered]
    small: /img/nue-page.png
    large: /img/nue-page-big.png
    caption: "Nue: content is fully extracted for copywriters"
    href: //github.com/tipiirai/nue/blob/master/new-www/index.md?plain=1


### UX developers
The whole point of a web framework is to help build user-friendly websites that look great. But today, this is all too complex. The user experience developers must know an awful lot of details about React, and TypeScript, even to render a simple "Hello, World" demo.

Nue is different: it brings back to the lost art of UX development, currently overshadowed by engineer-minded people who think that CSS is a terrible language that should not exist. Nue is the opposite: it's for people who love design, UX development, and the power of modern CSS.


### JavaScript developers
If you're a programmer or a backend engineer trying to learn the frontend stack, you are faced with an awful of new concepts and domain-specific idioms. What used to be plain and clean TypeScript is suddenly mixed with mysterious front-end coding.

Nue changes this completely. It separates your application from the front end so you can focus solely on your application logic. Just pure, type-safe code without the frontend spaghetti, which naturally belongs to the UX developer.

[image.gridpaper]
  small: /img/scale.png
  large: /img/scale-big.png


To sum up: Nue is not just another JavaScript framework. It increases the quality of your product and makes happier, more productive teams. You might not believe that until you actually try it out and experience the simplicity firsthand. You start wondering why you ever built frontends any other way.


- - -


## Continue reading

[.grid item="card"]
  ### Global Design System
  A universal styling framework for your web projects

  [Learn more](global-design-system.html)
  ---

  ### Content Management System
  A simple content management system for non-technical people

  [Learn more](content-management-system.html)
  ---

  ### Reactivity layer
  Turns your content into a rich, interactive experience

  [Learn more](reactivity.html)
  ---

  ### Single-page Applications
  Content-first development model for single-page apps

  [Learn more](single-page-applications.html)
