# JAM Milestone Delivery 


## Company/Team details

- Company/Team's name: Vinwolf
- Company/Team's GitHub: https://github.com/bloppan/
- Programming language and language set: Rust, set B
- Link/s to previous delivery/ies: None


## Documentation checklist

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **a clear Git history and public, credibly timestamped commits** 
- [x] we used third party libraries for: **cryptographic primitives** (ark-vrf, sp_core), **database** (rocksdb) and **networking** (quinn, tokio, rustls).
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [x] we have **not** had private conversations with **other implementers**.
- [x] we have **not** had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

This deliverable corresponds to M1 (Importer) of the JAM protocol, implemented in accordance with Gray Paper version 0.7.2.

This implementation was developed entirely by me, Bernardo López.

Vinwolf is an implementation of JAM written in Rust that I started in July 2024, and which I have developed progressively, incorporating both the required protocol specifications and the subsequent updates that have emerged as the specification has evolved.

The implementation covers all the logic required for correct block importation, including parsing, verification, and the state transitions defined by the protocol. At present, Vinwolf successfully passes all published test vectors and all available conformance traces.

Since August 2025, I have actively participated in all testing rounds conducted during the development of the fuzzer, which has contributed to strengthening the implementation and improving its robustness by identifying relevant edge cases.

In addition to the logic strictly required for M1, I have also implemented part of the networking logic that will be required for M2.


## Deliverables

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.


| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1.	      |Vinwolf source code	        | https://github.com/bloppan/vinwolf	   |Jam implementation   |
|2.	      |Binary target	        | https://github.com/bloppan/conformance_testing	   |Conformance testing (fuzz)    |
|3.	      |...	        | ...	   |...    |
|4.	      |...	        | ...	   |...    |
|5.	      |...	        | ...	   |...    |


## Additional Information

Without a doubt, this is the most interesting and demanding project I have worked on to date.

It has been developed entirely in my free time and represents my first blockchain development project, allowing me to acquire a substantial amount of valuable technical and conceptual knowledge.

Throughout the development, the primary focus has always been correctness and fidelity to the specification, prioritizing a clear and verifiable implementation over premature optimizations. 

