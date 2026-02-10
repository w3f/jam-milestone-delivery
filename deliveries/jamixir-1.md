
# JAM Milestone Delivery 


## Company/Team details

- Company/Team's name: WAGBI Consulting LLC
- Company/Team's GitHub: https://github.com/jamixir
- Programming language and language set: Elixir (Set D)
- Link/s to previous delivery/ies: N/A


## Documentation checklist

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **a clear Git history and public, credibly timestamped commits**.
- [x] we used third party libraries for: **cryptographic primitives** (blake2_elixir, ark-vrf, ring-proof, ark-ec, ark-serialize
, ed25519-zebra, reed-solomon-simd) and **networking** (quicer, X509).
- [x] we have **not** viewed any **JAM implementation code** before | during our implementation.
- [x] we have **not** had private conversations with **other implementers**.
- [x] we have **not** had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.

## Context

This submission delivers **Milestone 1 (IMPORTER)** of the JAM specification, based on Graypaper v0.7.2, implemented in Elixir as part of the Jamixir project.

The primary goal of this milestone is to demonstrate correct **state-transition conformance** and the ability to **import JAM blocks** according to the specification. All required conformance tests for the importer pass successfully.

During development, the team initially implemented the PVM in Elixir. While functionally correct, this approach revealed performance limitations. To prepare for future milestones, the PVM was subsequently re-implemented in Rust and integrated with the Elixir codebase via Erlang NIFs. This work is foundational and supports future performance-oriented milestones.

### Team
 - Daniel Cukier (@danicuki)
 - Baruch Fishman (@daiagi) - aka Luke

## Deliverables

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.

| Number | Deliverable                         | Link                                                  | Notes                                                        |
| ------ | ----------------------------------- | ----------------------------------------------------- | ------------------------------------------------------------ |
| 1      | Binary block importer (fuzzer)      | https://github.com/jamixir/jamixir-releases/releases  | Used for validating block import and robustness              |
| 2      | Jamixir core implementation         | https://github.com/jamixir/jamixir/releases/tag/0.7.2 | Elixir-based JAM implementation (commit tagged)              |
| 3      | Elixir PVM (initial implementation) | https://github.com/jamixir/jamixir-vm                 | Functional reference implementation                          |
| 4      | Rust PVM (performance-oriented)     | https://github.com/jamixir/pvm-rust                   | Integrated via Erlang NIFs; groundwork for future milestones |

## Additional Information

Working on JAM has been a significant learning experience for the team. While neither team member had prior experience building a JAM-class blockchain system, the formal specification proved to be precise and approachable. In particular, the mathematical rigor of the Graypaper maps naturally to Elixir’s functional paradigm.

We believe Jamixir will serve not only as a viable future JAM node implementation, but also as a valuable educational reference for developers seeking to understand JAM and its underlying design principles.
