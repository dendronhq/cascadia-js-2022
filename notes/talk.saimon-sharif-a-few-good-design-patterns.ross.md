---
id: 76i8e04c8dssvuo9oovt7np
title: Ross
desc: ""
updated: 1662069220193
created: 1662068347421
---

## a few good design patterns

**Saimon Sharif**

- EM at Attune

---

- origins from Gang Of Four - Design Patterns book

  - book contained 23 design patterns

- community has different reactions to design patterns

  - some seem very obvious
  - may seem too complicated
  - dynamic languages, eg JS, have different requirements/constraints than Java/etc

- useful to turn implicit knowledge into explicit

  - helpful to name concepts - provides a common language
  - code reviews

- hypothetical example - notepad startup pivoting to NFTs

  - going to add 90% discount - add abiity to enable/disable without deploying
  - solution: feature flag

- feature flag lets us enable/disable things without deploying, enable fast rollbacks & gradual releases

  - some vendors have admin panels to facilitate this
  - rolling your own feature flag service is a can of worms, don't do it - bad past experiences

- scenario: feature flag library creates a new websocket connection everytime feature is enabled

  - solution: use Singleton, ensure only one connection is created
  - singletons useful for accessing shared resources - files, database, cache

- scenario: add observability to getPrice() function

  - using performance API to measure execution time
  - would need to change all code to wrap w/calls to performance API
  - solution: use decorator pattern to annoitate functions to be instrumented
  - decorators - still TC39 proposal, available in Typescript
  - decorators are easy to add/remove

- scenario: getFavorites() function does DB stuff, needs caching

  - would like to add caching anywhere in a generic way
  - solution: use Proxy pattern
  - proxies allow us to control access to an object; we'll use to return cached value
  - built-in to Javascript, though syntax is a bit hairy
  - example of caching Math.random
  - result is clean & simple w/separation of concerns

- scenario: CEO wants to launch duplicate NFTs/object feature
  - like JQuery or Knex - method chaining, use their own DSL
  - solution: fluent interfaces
  - our own version of method chaining

---

- two ways of learning
  - just-in-time vs just-in-case
  - neither better, good to know your bias
  - try the opposite of your normal way of learning
