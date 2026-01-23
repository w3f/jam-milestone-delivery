# JAM Milestone Delivery 


## Company/Team details

- Company/Team's name: Chainscore
- Company/Team's GitHub: https://github.com/chainscore
- Programming language and language set: Python (Set D)
- Link/s to previous delivery/ies: N/A (First milestone)


## Documentation checklist

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**. (GPL-3.0-only)
- [x] we submitted **a clear Git history and public, credibly timestamped commits**.
- [x] we used third party libraries for: **cryptographic primitives** (e.g. erasure-coding, Bandersnatch, Ed25519) | **codecs** (e.g. SCALE) | **networking** (e.g. QUIC).
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation: None
- [ ] we have not had private conversations with **other implementers**.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.


## Context

Tessera is a clean-room JAM client implementation in Python. This milestone demonstrates that Tessera can successfully import blocks and pass state-transitioning conformance test vectors as specified by W3F.

## Deliverables

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.


| Number | Deliverable | Link | Notes |
|--------|-------------|------|-------|
|1. | Source Code | https://github.com/chainscore/tessera | JAM client implementation in Python |
|2. | Releases | https://github.com/chainscore/tessera-releases | Binary releases and distribution packages |

## Additional Information

Our code repository is public since Nov 2025. During development, commit hashes were regularly anchored and published to a public blockchain here - https://polygonscan.com/address/0x0113e1920540fa9547389d02e7e79f60b4d4f503#events