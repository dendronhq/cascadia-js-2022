---
id: hdjnyz8eg83xbgodnhyjcd3
title: courier-new
desc: ""
updated: 1662074465010
created: 1662074096091
---

## Intro

- Dynamic languages will benefit from different design patterns from static or compiled languages
- Why care about design patterns? Knowing the name for a concept gives us a common language to discuss them with.

## An opinionated list of good design patterns

...Some of which come from the [Design Patterns](https://www.digitalocean.com/community/tutorials/gangs-of-four-gof-design-patterns) book by the Gang of Four.

### Feature Flags

- Not a “traditional” design pattern
- Enable fast rollbacks and gradual releases

### Singleton

- Guarantee a given class only has one instance while making that instance globally available
- Enable access to a shared resource (file, DB, web socket, etc.)

### Decorator

- Attach instrumentation (such as tracing) to another function
- TS has first-class [decorators](https://www.typescriptlang.org/docs/handbook/decorators.html)
- TC39 has [stage 3 proposal](https://github.com/tc39/proposal-decorators) for decorators
- Multiple types: method decorator, class decorator

### Proxy

- Enables controlling access to an object
- Built-in `Proxy` in JS: `new Proxy(obj, handler)` where handler intercepts and redefines what methods (such as `obj.get` should return)
- [Mozilla docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Proxy)

### Fluent Interface

- An object-oriented API that relies on method chaining
- Increase code legibility and composability with a domain-specific language

## Ending thoughts

Consider if you’re more of a just-in-time learner or a just-in-case learner, and give the other type a try sometime!
