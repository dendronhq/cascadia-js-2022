---
id: ian-sutherland
title: Zero-dependency CLIs with Node.js
desc: ''
updated: 1662050842794
created: 1661898027712
tags:
  - node-js
  - cli
  - javascript
location: 'Calgary, AB, Canada'
uri: ''
twitter: iansu
company: Neo Financial
pronouns: he/him/his
enableGiscus: true
---
> The contents here is created from the official [CascadiaJS Page](https://2022.cascadiajs.com/speakers/ian-sutherland)

## Overview

![Ian Sutherland image](https://create-4jr.begin.app/_static/2022/ian-sutherland.jpg){max-width: 300px}
- name: Ian Sutherland
- [Speaker Page](https://2022.cascadiajs.com/speakers/ian-sutherland)

## Abstract

Node.js is a popular choice for building dev tools and some recently added features make it possible to build powerful tools without any external dependencies. We’ll look at these new features and show how to use them to build a custom CLI app with zero external dependencies.

## Notes

![[talk.ian-sutherland-zero-dependency-clis-with-node-js.*]]

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
