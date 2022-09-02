
### Notes by [kevin](https://github.com/kevinslin)

- javascript engine
	- multiple engines: v8, spidermonkey, apple jscriptcore
- v8 executes js in context
	- ecmascript web specs not part of v8
	- chromium embeds v8 and provides DOM apis
	- node embeds v8 and provides system apis
	- ruby racer embeds v8 to call js from ruby
- v8 does not just interpret js
	- many parts
		- parse, optimization, codegen
		- turbofan: part that optimize code
- optimizing
	- what v8 mainly optimizes
		- inlinable functions 
		- function with stable signature
- functions example
  - #todo
- objects example
	- getObject 1e6 times
	- to optimize object, requires
		- same fields with same type
		- types crated in same order
	- calling same object initialized with object of different order will stop optimizations
- native funciton syntax `%`
	- run v8 with `--allow-native-syntax`
	> TIP: you can set v8 flags inside nodejs
	- native syntax are undocumented v8 apis, used for testing and debugging
		- you can find the v8 source
		- docs are in v8 tests
	- can used to manipulate optimization (eg. never optimize this function)

- what can i do with native functions?

- question1: are optimized functions faster?
	- benchmarkjs to test
- question2: check optimization status of a function within code
	- print to debug
	- if you keep opt/de-opt function, v8 will give up on your code 
- question3: can i manipulate memory related stuff
	- yes, but please do it

- how does devtools work
	- chrome debug protocol
		- websockets
		- communicate with v8/chromium
		- access debug interface:
  		- debugger
  		- heap profiler
  		- cpu profiling/code coverage
  		- dom (browser only)
			- eg. playwright uses this
			- eg. remote debug node
		- gives access to **everything** in node process

- debug protocol
  - cpu profiling is polling based
	- control polling rate from protocol (not available in dev tools)
- heap profiler
	- show everything in heap
	- eg. find memory leak

- why
	- remote debugging
	- atuomated diagnostics
	- script debugging
		- eg. add breakpoint
		- execute code and check heap
		- canbe used in extensions

- other topics
	- v8 inlining
	- torque language
	- v8 treats web assembly
	- how v8 manages strings
	- etc
	- most of this is on https://v8.dev/

## Notes by [aminamos](https://github.com/aminamos)
- v8 is a JS engine
    - the engine takes JS code as an input and executes it
- v8 is one of many engines
- DOM manipulation APIs are not defined in v8
- node embeds v8 and has JS APIs
- v8 is embedded (ruby, deno examples)
- turbofan, sparkplug, ignition
- [discussion around code optimiziation, de-optimization, re-optimization]
- are optimized functions better? yes
- can I check optimization status of a function in the code? yes
- chrome debug protocol convo, CPU profiling is polling based (and this rate is configurable)
- can get heap dump, then dig into info in dev tools (all objects, all streams that are currently alive)
- other toppics
    - v8 code inilining, WebAssembly, string management, torque language, v8 snapshots
    - check out https://v8.dev/
