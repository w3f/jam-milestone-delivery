# JAM Milestone Delivery

## Company/Team details

- Company/Team's name: SpaceJam
- Company/Team's GitHub: [https://github.com/spacejamapp](https://github.com/spacejamapp)
- Programming language and language set: Rust / Set B
- Link/s to previous delivery/ies: _none_

## Documentation checklist

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **a clear Git history, credibly timestamped commits in a private github repository**
- [x] we used third party libraries for:
  - **cryptographic primitives**: `ark-*`, `blake2`, `ed25519-zebra`, `tiny-keccak`, `w3f-bls`, `w3f-ring-proof`, `rcgen`
  - **networking**: `quinn`
  - **encoding**: `reed-solomon`, `serde`
  - **storage**: `parity-db`
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [x] we have not had private conversations with **other | the following implementers**.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the _Polkadot Technical Fellowship_ on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the _Polkadot Technical Fellowship_ before it can be merged.

## Context

SpaceJam has successfully passed all test vectors:

- [0.7.2 jam-conformance vectors](https://github.com/davxy/jam-conformance)
- [0.7.2 jam-test-vectors](https://github.com/davxy/jam-test-vectors)

We have the best performance overall third-parity implementations according to [jam-conformance-dashboard][perf].

- We have developed our [PVM compiler][spacevm] which supports both AOT & JIT compilations.
- We have developed the [Jade Framework](https://github.com/spacejamapp/jade) for writing PVM programs.
- We have developed [PVM Codes][codes] for people learning PVM.
- We have developed a JAM explorer (currently got offline due to the delay of M1)

## Deliverables

- [x] 1. Validating Node Path
- [ ] 2. Non-PVM Validating Node Path
- [ ] 3. Light Node Path

- **Milestone:** 1

| Number | Deliverable              | Link                             | Notes                           |
| ------ | ------------------------ | -------------------------------- | ------------------------------- |
| 1.     | SpaceJam binaries for M1 | [releases/0.7.2][v0.7.2]         | the binaries are at GP-0.7.2    |
| 2.     | SpaceJam source code     | [spacejamapp/spacejam][spacejam] | This is currently not public    |
| 3.     | Jade Framework           | [spacejamapp/jade][jade]         | For writing PVM programs        |
| 4.     | SpaceVM ABI              | [spacejamapp/spacevm][spacevm]   | sys library for calling SpaceVM |
| 5.     | PVM Code tables          | [pvm-codes][codes]               | website for learning PVM        |

[v0.7.2]: https://github.com/spacejamapp/specjam/releases/tag/0.7.2
[spacejam]: https://github.com/spacejamapp/spacejam
[jade]: https://github.com/spacejamapp/jade
[perf]: https://github.com/paritytech/jam-conformance-dashboard
[spacevm]: https://docs.rs/spacevm-sys/latest/spacevm_sys/
[codes]: https://pvm.spacejam.app/
[clearloop]: https://github.com/clearloop
