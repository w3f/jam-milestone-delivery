# JAM Milestone Delivery 

## Company/Team details

- Company/Team's name: Colorful Notion 
- Company/Team's GitHub: 
  - https://github.com/colorfulnotion/jam (code)
  - https://github.com/jam-duna/jamtestnet/releases (Fuzzer Target)
- X: [https://x.com/colorfulnotion](https://x.com/colorfulnotion)
- Programming language and language set: Go (Set A), supported by C (recompiler) + Rust (BLS/Bandersnatch FFI)

Team members:
* [Sourabh Niyogi](https://github.com/colorfulnotion/jam/commits?author=sourabhniyogi) (active, Summer 2024-present)
* [Michael Chung](https://github.com/colorfulnotion/jam/commits?author=mkchungs) (active, Summer 2024-present)
* [Shawn Chung](https://github.com/colorfulnotion/jam/commits?author=yoyo2325) (active, Fall 2024-present) 
* Tapas Jana (active, Fall 2024-present, eng support)
* William Wu, Stanley Liu, Sean Tsu (inactive, Fall 2024 - Winter 2025)


## Documentation checklist

We declare that:

- [ ] we have completed **the Web3 Foundation KYC/KYB process**.
- [X] we used **a clear and permissive open-source license**.
- [X] we submitted **a clear Git history and public, credibly timestamped commits** | **code developed in private, with commit hashes placed, in a timely fashion, on a major public blockchain**.
- [X] we used third party libraries for: **cryptographic primitives** (bls, simd)) | | **networking** (quic-go).
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code**  our implementation.
- [X] we have not had private conversations with other implementers.  See here for disclosures.
- [X] we have not had **concerns about collusion**.
- [X] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [X] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.

## Context

JAM DUNA implements the JAM protocol as of GP 0.7.2.  Written in Go (with FFIs into Rust W3F libraries for bls/safrole + Erasure coding) and supported by a C PVM X86 Recompiler (originally in Go), our implementation aims to be a highly performant production-grade implementation that leading JAM validators can use to secure trustless supercomputing in the coming years. Our history over the last year is documented [here](https://github.com/jam-duna/jamtestnet?tab=readme-ov-file#history).

Our implementation has successfully passed @davxy test vectors sets:

 - [0.7.2 jam-conformance vectors](https://github.com/davxy/jam-conformance)
 - [0.7.2 jam-test-vectors](https://github.com/davxy/jam-test-vectors)

From [jam-conformance-dashboard](https://paritytech.github.io/jam-conformance-dashboard/) we believe our target provides adequate performance for sustained W3F testing in January 2026.

Our team has developed prototype EVM smart contract interpretation services using polkatool along with a battery of other test services (see [colorfulnotion/polkavm](https://github.com/colorfulnotion/polkavm/tree/dev/services)) and a Go+C-based recompiler, enabling high performance multi-core GGas/s EVM execution.   

We have participated in in-person + online events where we have met many in the JAM community
 * Nov 2025 JAM0 meetup in Bangkok (organized by me)
 * May 2025 JAMXP Lisbon + JAM Toaster preview
 * May 2025-Aug 2025 JAM DAO Decentralized Voices
 * Telegram => Discord implementers channel

Other accomplishments: (WIP, to be made increasingly conformant in 2026)

- [x] JAM-NP UP0/CE128..153 (PoC, tested against Polkajam with Doom WPs and our EVM WPs)
- [x] Functioning Recompiler (PoC)
- [x] Auditing + GRANDPA (PoC)
- [x] Doom WP Refinement (PoC -- work report matches except for one byte)

We fully intend to engage in the full validator path [M3, M4, M5] in 2026-2027 and hope to eventually be a
buyer of CoreTime of Polkadot JAM someday in having sustainable trustless supercomputing services.  

## Nominations

We propose the following for Fellowship membership in M1:

* [Michael Chung](https://github.com/mkchungs)
* [Shawn Chung](https://github.com/yoyo2325) 

Both can actively contribute to JAM's evolution and development with others in the Polkadot/JAM community.

## Deliverables

- [X] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.

| Number	| Deliverable	         | Link	 | Notes                                          |
|---------|----------------------|--------|------------------------------------------------|
|1.	      | 0.7.2 Fuzzer target	 | [github.com/jamduna/jamtestnet](https://github.com/jam-duna/jamtestnet/releases)	   | |
|2.	      | JAM DUNA source code | [github.com/colorfulnotion/jam](https://github.com/colorfulnotion/jam)	   | Currently private -- Access granted to W3F / Fellowship upon request                       |
|3.	      | JAM DUNA Commit history	 | [Subscan](https://assethub-polkadot.subscan.io/extrinsic?module=system&call=remark_with_event&signed=all&page=1&time_dimension=date&address=121Rs6fKm8nguHnvPfG1Cq3ctFuNAVZGRmghwkJwHpKxKjbx)	   | ...                                            |
|4.	      | ...	                 | ...	   | ...                                            |
|5.	      | ...	                 | ...	   | ...                                            |

## Acknowledgements

We are deeply grateful to Gavin Wood, Davide Galassi, Dave Emmett, Jan Bujak, Jeff Burdges and many others in the JAM Implementers community who have taught us so much and made the puzzle of trustless supercomputing so rewarding process over the last 18 months.  

