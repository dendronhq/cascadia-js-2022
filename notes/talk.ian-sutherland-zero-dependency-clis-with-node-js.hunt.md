---
id: qw65fj10qz0hw8aqu1255aq
title: Hunt
desc: ''
updated: 1662052395784
created: 1662050848362
---

- Neo Financial, Head of DEX and OSS
- twitter @iansu
- flags
    - `-l1` or `-l -1` Short options
    - `--color` Long options
- subcommands
    - the `status` in `git status`
- "CLI is serious 80s vibes"
- Node has a small core which is why there are lots of dependencies installed with `npm` for a given project like `isNumber`.
- Bundling isn't the best because it can still result in a large bundle size.
- `type: module` to package.json to use `import` and ESMM or us `.mjs` (as opposed to `.cjs`).
- import Node.js internals with `node:`
    - eg, `import fs from 'node:fs'`
- There are many different ways to set arguments in a cli
- parseArgs: `process.argv` -> Tedious so use `yargs` of `commander`.
    - NOT TEDIOUS ANYMORE!  `parseArgs from 'node:util'` uses `process.argsv`
        - declare the options (kind of like commander)
    - has polyfill, will be "backboarded" to v16
- fetch: now available in node@18
    - Built on top of Undici (HTTP/1.1)
- see `iansu/git-blast` on github to run git blast and see people's twitter handle's if supplied on githu
- node@18 now has a basic test runner.
    - don't necessarily need jest anymore.
    - `node --test`
- recursive mkdir function with `{recursive: true}`
- recursive rm operation `{recursive: true, force: true}`
- recursive cp (same as mkdir) **experimental
- readdir **open pr, not merged
- Speculation of what's next
    - glob patterns
    - self contained executables
    - native typescript (aka deno)

[build the future](https://github.com/nodejs/tooling)
