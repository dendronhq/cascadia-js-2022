
### Notes by [kevin](https://github.com/kevinslin)

- speaker
	- three-vikram
	- #CascadiaJS
- publishing
	- browsers: 
	- servers: nodejs, deno, etc
	- ns native: react, native, flutter
	- module formats: cjs, esm
	- sizes: publish, install, bundle
	- types: flow, typescript
	- debugging: source, sourcemap
	- observability: open*, etc
- criteria to consider
	- depends
- publishing criteria
	- why, how, what

- browser, why?
	- script on browser
	- isn't js support fragmented on browser
	- yes but
		- IE retired in 05/15/2022
		- safari competitive? (lol)

- server, why
	- nodejs most popular
	- deno
	- fragmentation?
		- web interoperable runtimes community group

- deno, how?
	- experimental npm support

- bun, how?
	- compatible?

- js native, why?
	- write javascript, ui framework create native apps
	- have limitation
	- perf tradeoffs, has become better

- module formats, why?
	- ...


- module formats, how?
	- supporting cjs/esm, you can use esm module wrapper
	- `gen-esm-wrapper`

- sizes (why)?
	- publish: pkg being published
	- install: `node_modules` on install
	- bundle: bundled artifact

	- why important?
		- load times
		- constrained environments (eg. serverless)

- reducing size
	- publish:
		- remove unecessary things in package.json
			- eg. move types to definitely typed
	- install
		- minimal dependencies
		- provide variant of pkg for resource-constraint environment
	- bundle
		- tree-shakeable code
			- named exports
		- publish esm version of pkg
		- remove side effects

- types (why)
	- ts popular
	- ecmascript proposal for type annotation

- debugging (why)
	- you have a language that compiles to js
		- source maps for debug

- observability (why)
	- help measure state of app

- observability (how)
	- add opentelemetry package

- conclusion
	- brwoser: support modern browser
	- server: nodejs with deno support
	- js native: depends
	- module formats: cjs+esm or esm only
	- sizes: aim small
	- types: publish typescript types
	- debuggign: provide sources
	- observability: add hook to open telemetry