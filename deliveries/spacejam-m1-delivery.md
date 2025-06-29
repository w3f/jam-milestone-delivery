# JAM Milestone Delivery

## Company/Team details

- Company/Team's name: SpaceJam
- Company/Team's GitHub: [https://github.com/spacejamapp](https://github.com/spacejamapp)
- Programming language and language set: Rust
- Link/s to previous delivery/ies: _none_

## Documentation checklist

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **a clear Git history and public, credibly timestamped commits** | **code developed in private, with commit hashes placed, in a timely fashion, on a major public blockchain**.
- [x] we used third party libraries for:
  - **cryptographic primitives**: `ark-*`, `blake2`, `ed25519-dalek`, `tiny-keccak`, `w3f-bls`, `w3f-ring-proof`
  - **networking**: `quinn`, `rcgen`, `tokio`, `jsonrpsee`, `axum`
  - **encoding**: `reed-solomon`, `serde`
  - **storage**: `parity-db`
- [x] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [x] we viewed the following **JAM implementation code** before | during our implementation.
- [x] we have not had private conversations with **other | the following implementers**.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the _Polkadot Technical Fellowship_ on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the _Polkadot Technical Fellowship_ before it can be merged.

## Context

1. we can pass [all trace tests](https://github.com/w3f/jamtestvectors/tree/master/traces) at `0.6.6`.
2. we have introduced a fuzz target in the [spacejam](https://github.com/spacejamapp/specjam/releases/tag/0.6.6) binary at `0.6.6`.

## Deliverables

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.

| Number | Deliverable                | Link                             | Notes                         |
| ------ | -------------------------- | -------------------------------- | ----------------------------- |
| 1.     | spacejam binary at `0.6.6` | [releases/0.6.6][v0.6.6]         | spacejam binaries at GP-0.6.6 |
| 2.     | spacejam source code       | [spacejamapp/spacejam][spacejam] | This is currently not public  |

## Additional Information

[v0.6.6]: https://github.com/spacejamapp/specjam/releases/tag/0.6.6
[spacejam]: https://github.com/spacejamapp/spacejam
