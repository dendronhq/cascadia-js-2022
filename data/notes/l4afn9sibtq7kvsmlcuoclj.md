

### Notes by [kevin](https://github.com/kevinslin)


- dependencies breaking is bad
- Browsers broke stuff all the time back in the day, most browsers are backwards compatible now.
- Build around what will not break in the next 10 years, not what you think will change.
- additive changes help with not breaking things
  - http1 -> http2
  - xml http request -> fetch
  - async/await
  - `<script type="module"></script>`
  - woff -> woff2
  - s3.listobjectsv2
- lots of moving parts
- Can we simplify? Yes! [progressive enhancement](https://en.wikipedia.org/wiki/Progressive_enhancement)
  - Start working with HTML and add JS on top of that.
  - good for accessibility, audience usage and also help with dependencies
- framework are incorporating this
  - [11ty](https://www.11ty.dev/), [remix](https://remix.run/), [astro](https://astro.build/)

Enhance is a project built in the HTML first, JS and CSS on later manner.
- api routes
- its kind of like php, not a bad thing
- file based routing with plain html
- reuse markup wtih custom elements
- built-in utilities
- uses pure functions to return HTML components

 - Poor Man's Debugger - `JSON.stringify(state, null, 2)`