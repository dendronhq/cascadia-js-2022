
- works at chainguard using kuberneties

- don't roll your own cryptography
- RSA isn't the bees knees anymore

- Modular Arithmetic
    - "one way door"
- Eliptic Curve Cryptography
    - also one way door.  AFAIK it's the backbone of blockchain
    - `y^2 = x^2 + ax + b`
    - used in the generation of a public and a private key
- Diffie Hellman Key Exchange
- `import crypto from 'node:crypto`
    - Sample Diffie Hellman Key Exchange code sample...
- `getRandomValues(TypedArray)`, `randomUUID()`, `subltle`
    - Why subtle?  Easy to shoot yourself in the foot.
- NSA's cryptography function scandal `Dual_EC_DRBG`.
    - require usage of P and Q
    - NSA knows `e`?
- https://sigstore.dev
    - OSS
    - Let's Encrypt for signing
    - Fulcio: keyless signing
    - Rekor: transparency log
    - Cosign: Container signing
    - A tool for signing and verifying npm packages
- npm RFC 626: linking packages to source and build
    - proof of where package was built

## Presentation Notes

- full of nice gif memes.

[slides](https://bit.ly/3pZwLzG)

Recommends the [computerphile youtube channel](https://www.youtube.com/user/Computerphile).