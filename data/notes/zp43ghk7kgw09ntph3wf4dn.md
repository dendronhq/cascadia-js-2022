
### Notes by [kevin](https://github.com/kevinslin)

- disclaimer: don't try this at home

- symmetric keys: everyone has key
- asymmetric key (public key cryptography): only share public key
- one way functions: hard to reverse operation
- pseudorandom number generators: sources of entrophy
- rsa
	- great when it came out, not recommended anymore
- modular arithmetic
	- % operator in javascript
- elliptic curve cryptography (ecc)
- why ecc
	- rsa needed to increase bit length to make stronger
	- ecc scales better
- diffie hellman key exchange
	- agree over symmetric key in insecure channel
	- eg. ssh 
- web crypto api
	- built into browser
- nsa backdoor
	- pseudo random number generator that is broken by design
	- believed that nsa has backdoor
- sigstore
	- new standard for signing, verifying, and protecting software
	- lets encrypt for signing
