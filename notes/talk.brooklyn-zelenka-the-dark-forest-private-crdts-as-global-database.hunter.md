---
id: vpqdoglqn3m55o8pdeat6gu
title: Hunter
desc: ''
updated: 1662078475663
created: 1662076871980
---

- @expede
- Fission Codes
- WNFS, Dialog, CAR Pool, PVM

- Keeping data in a database is a bad idea.  See GDPR.
    - If you don't store data you can't be persecuted for storing any data you shouldn't.

- Networked Data, not apps
    - Stuff comes first

- Open protocols
    - Auth: interop without pre-negotiation
    - Data
    - Compute

- Global Primary Keys
    - Content addressing
        - Truly global links as opposed to ip addresses (physical location), DNS, networked routing for hashed data, 
        - Hard links vs soft links (url)
        - Content IDs (CID)
        - Seems to basically just be like a REST request, but instead of using an id, just use the hash of the object
            - What do you do when you update the data, wouldn't its hash be updated?
                - Brooklyn explains this.  All history is needed (wink wink blockchain)
- Portable Private Data
    - SublteCrypto(Web Crypto)
        - Never gives direct access to the key
        - Add an ownership node to the object
- BFT Concurrency
    - Over my head, something about color mixing, commutability, associative, and (does not change f(x) === f(f(x)));
- See also CRDT