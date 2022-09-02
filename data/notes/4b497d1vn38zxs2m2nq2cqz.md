
### Notes by [kevin](https://github.com/kevinslin)

- cli apps
	- stuff that runs on the terminal
- features
	- options (eg. `ls`)
	- subcommands (eg. `git`)
- why node
	- scripting language
	- good at json, parallel task, network request, etc
	- lots of packages
- dependencies
	- other code (eg. library)
	- node does not have big standard lib
- are deps bad?
	- depends
	- does introduce overhead
	- you can bundle to make it better
- new syntax
	- using `import` (es module)
	- import nodejs internals with `node:` prefix
		```js
		import fs from "node:fs"
		```
	- every npm name is taken, we couldn't add anything new, hence new namepsace
- argument parsing
	- old way:
		```js
		// get everything from STDIN, split by whitespace
		// eg. [node, mycli, --ls]
		const args = process.argv
		```
- argument parsing
	```js
	import {parseArgs} from "node:util"
	const input = process.argv.slice(2)
	const options = {
		silent: {
			type: 'boolean',
			short: 's'
		}
	}
	const {values} = parseArgs({input, options}):
	```
- fetch
	- make http request
	- its available in **node 18**
	- built on top of undici (http/1.1 client)
	- has web streams api
	```js
	// available globally
	const response = await fetch("...")
	const body = await response.json()
	// you get JSON
	{
		...
	}
	```

- demo to add new git subcommand the old way
	```js
	// very long example
	// ...
	```

- demo with new way
	```js
	// very short example (less than 10 lines)
	// ...
	```

- test runner
	- basic api to do this
	- eg. mocha but builtin to node
	```js
	import test from "..."
	test("synchornous test", (t) => {
		//...
	})
	// also works async
	```

- recursive file system ops
	```js
	import {rm} from "node:fs/promises"

	// experimental 
	import {cp} from "node:fs/promises"

	// doesn't exist yet, open pr
	import {readdir} from "node:fs/promises"
	```

- whats next
	> DISCLAIMER: complete speculation

	- glob?
	- self contained executable
	- typescript (lol - i wish)