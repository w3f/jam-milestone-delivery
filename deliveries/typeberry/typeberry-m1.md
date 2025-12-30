# JAM Milestone Delivery 

## Company/Team details

- Company/Team's name: Fluffy Labs
- Company/Team's GitHub: https://github.com/FluffyLabs
- Programming language and language set: TypeScript / AssemblyScript (Set C)
- Link/s to previous delivery/ies: -


## Documentation checklist

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
  KYB as Fluffy Labs sp. z o.o.
- [x] we used **a clear and permissive open-source license**.
  Mozilla Public License 2.0
- [x] we submitted **a clear Git history and public, credibly timestamped commits** | **code developed in private, with commit hashes placed, in a timely fashion, on a major public blockchain**.
  - Repository at https://github.com/FluffyLabs/typeberry (public since Sep 2025)
  - Commit history confirmation https://assethub-kusama.subscan.io/account/EJxhMZtb2QJdJ5qnLegyqY7TQPpLgG9rNxXiBxmEkPAk4DH
- [x] we used third party libraries for:
  - bandersnatch: Rust `ark-vrf` compiled to WASM (https://github.com/FluffyLabs/typeberry-native/)
  - ed25519: Rust `ed25519-consensus` compiled to WASM (https://github.com/FluffyLabs/typeberry-native/) for verification
  - ed25519: NPM `@noble/ed25519` for public key derivation and signing
  - keccak: NPM `hash-wasm`
  - blake2b: NPM `hash-wasm`
- [x] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
  - N/A
- [x] we viewed the following **JAM implementation code** before | during our implementation.
  - none
- [x] we have not had private conversations with **other implementers**.
  - no conversations about the implementation itself
- [x] we have not had **concerns about collusion**.
  - N/A
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.


## Context

Since September 14th we are actively participating in the fuzzing rounds (see https://github.com/davxy/jam-conformance/issues/81).
To our best knowledge, the implementation also passes all available test vectors for M1 conformance.

## Deliverables

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.


| Number  | Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1.	      | Source Code     | https://github.com/FluffyLabs/typeberry	                        | JAM fuzz target & client source code  |
|2.	      | Docker image    | https://github.com/FluffyLabs/typeberry/pkgs/container/typeberry  | Fuzz target & client |
|3.	      | NPM package     | https://www.npmjs.com/package/@typeberry/jam                      | Fuzz target & client |


## Additional Information

>Provide any relevant comments on the milestone submission that you would like to share with us.




