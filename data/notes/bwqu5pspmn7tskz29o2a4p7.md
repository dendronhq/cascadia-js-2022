

- There were many design patterns and pattern languages before the Gang of Four was released.
- Calls Hacker News the "orange website". 
- Works as an engineering manager at Attune
- Design Patterns are *obviously* worthwhile.
- How to enable and disable a discount without needing to redeploy?
    - Feature flag: allow disabling and enabling things without deploying
        - Fast rollback
        - Gradual releases
        - "don't roll your own feature flag"
    - Singleton pattern to fix an issue with a websocket being made every time a feature flag is set (?)
        - calls the singleton `static #<name> = null` <<using a variable name starting with a #>>.
    - Trace function -> Heatmap
    - Decorator pattern: wrap object and add new bheavior to those objects.
        - easy to remove, since you can easily remove the line of code
    - Proxy pattern
        - controls access to an object
        - returns a cached vaalue
        - `Proxy` exists in JS
        - `new Proxy(obj, handler)`;
            - handler is an object with a function "get" used to trap the return value
            - [mdn proxy docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Proxy)
    - Fluent interface
        -examples
            - knex query building
            - jquery
            - rxjs
        
