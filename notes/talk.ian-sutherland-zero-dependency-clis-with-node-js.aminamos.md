---
id: g9dnm5ogxwo4ehkjhzkaw4r
title: Aminamos
desc: ''
updated: 1662056648531
created: 1662056630340
---

## Notes by [aminamos](https://github.com/aminamos)
- topics
    - what is a cli
    - what are dependencies, why avoid them
    - what helps us write cli apps
    - new upcoming nodejs features 
- CLIs use flags/options
- why build with node?
    - usually a language your team is already familiar with
    - JSON data operations, network requests are pretty well supported
    - node has a package ecosystem (useful when needed, still avoid when possible)
- dependencies
    - code that your program needs to run
    - all users of your app will need to install dependencies
    - smaller apps, like  CLIs, not having an install or build step makes setup, contributing, and distribution easier
- new node syntax
    - import instead of require
    - ESM instead of CJS
- argument parsing
    - this process is surprisingly complicated
    - https://nodejs.org/docs/latest/api/process.html#processargv
    - third party library like yargs or commander, in the past
    - parseArgs is ~the future~ as of node 18.3 (potentially backported to node 16)
        - polyfill proposal for util.parseArgs() - https://www.npmjs.com/package/@pkgjs/parseargs
        - doesn't support all previous functionality, but useful error messages
        - https://nodejs.org/api/util.html#utilparseargsconfig
- fetch
    - before fetch, had to do a lot of pre-work to setup, run, and handle http requests
    - with fetch you can just `await fetch()` and return the body/errors
    - `git blast` is real https://github.com/iansu/git-blast
- test runner
    - https://nodejs.org/api/test.html#test-runner
- recursive file system operations
    - https://nodejs.org/api/fs.html#fspromisesmkdirpath-options
    - https://nodejs.org/api/fs.html#fspromisesrmpath-options
    - recursive copy
- wild speculation
    - self contained executibles
    - glob
    - typescript `node index.ts`
- what's next, ways to contribute
    - join node tooling group https://github.com/nodejs/tooling
