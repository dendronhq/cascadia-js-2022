---
id: 85jow1i5e8pisi4gtacixyz
title: Kevinslin
desc: ''
updated: 1662078043241
created: 1662076890089
---

### Notes by [kevin](https://github.com/kevinslin)

- speaker
	- cto of fission codes
	- working on lots of protocols
- context for auth 
	- theres a lot in th emiddle
	- lots of data is sensitive
- networked data, not apsp
- 3 techniques
	- global primary key (content hashing)
	- cryptrees/dark forest
- content hashing
	- never change
	- *hard links for the web*
	- self verifying data
- private data substrate
	- traditional: file system
	- new:
		- partitioned
		- persistent & versioning
			- feature but also implementation detail
			- just maps under the hood
		- private data
			- crypto is just transforming existing problems into key management problems
			- what changed: ubiquitous web crypto api 
				- you can't extract keys using the api, only signing
- offline access control
	- use hash tree vs trie
- concurrent writes