---
id: eddie-zaneski
title: Cryptography Isn't Scary
desc: ''
updated: 1661982729179
created: 1661898027709
tags:
  - cryptography
  - software-supply-chain
  - code-signing
location: 'Denver, CO, USA'
uri: ''
twitter: eddiezane
company: Chainguard
pronouns: he/him/his
enableGiscus: true
---
> The contents here is created from the official [CascadiaJS Page](https://2022.cascadiajs.com/speakers/eddie-zaneski)

## Overview

![Eddie Zaneski image](https://create-4jr.begin.app/_static/2022/eddie-zaneski.jpg){max-width: 300px}
- name: Eddie Zaneski
- [Speaker Page](https://2022.cascadiajs.com/speakers/eddie-zaneski)

## Abstract

Cryptography isn't scary, it's fun! Join for a crash course in modern cryptography. Learn what's available in Node and the browser along with how we are securing the software supply chain.

## Notes

![[talk.eddie-zaneski-cryptography-isn't-scary.*]]

## Notes by [aminamos](https://github.com/aminamos)
- symmetric, asymmetric, one-way functions, pseudorandom number generators
- RSA
    - time to phase this out
    - prime factorization
- modular arithmetic is a one-way function
- ECC elliptic curve cryptogrpahy
    - allows shorter key lengths but more security
- DHKE
- web crypto API https://developer.mozilla.org/en-US/docs/Web/API/Web_Crypto_API
- SubtleCrypto https://developer.mozilla.org/en-US/docs/Web/API/Web_Crypto_API
- Dual_EC_DRBG https://en.wikipedia.org/wiki/Dual_EC_DRBG
    - https://www.youtube.com/watch?v=nybVFJVXbww
- Sigstore - Let's Encrypt for signing
