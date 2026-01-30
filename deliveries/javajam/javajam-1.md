# JAM Milestone Delivery 

## Company/Team details

- Company/Team's name: JavaJAM
- Company/Team's GitHub: 
  - https://github.com/javajamio/
  - https://github.com/methodfive/javajam
- Project twitter: https://x.com/javajam_io
- Programming language and language set: Java (Set A)
- Link/s to previous delivery/ies: N/A

## Documentation checklist

We declare that:

- [X] we have completed **the Web3 Foundation KYC/KYB process**.
- [X] we used **a clear and permissive open-source license**.
- [X] we submitted **a clear Git history and public, credibly timestamped commits** | **code developed in private, with commit hashes placed, in a timely fashion, on a major public blockchain**.
- [X] we used third party libraries for: **cryptographic primitives** (reed-solomon-simd, ed25519-zebra, w3f-bls, Bandersnatch, bouncycastle for blake2b/keccak) | | **networking** (Netty QUIC).
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [X] we have not had private conversations with other implementers.
- [X] we have not had **concerns about collusion**.
- [X] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [X] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.

## Context

JavaJAM is an enterprise-grade implementation of the JAM protocol, created by Jason Mansfield, designed to support Polkadot’s JAM network with a strong focus on correctness, performance, and operational resilience. Built in Java, JavaJAM leverages the language’s security model, mature tooling, and platform independence to deliver a robust, event-driven architecture suitable for long-running, large-scale validator and worker deployments.

The implementation has successfully passed all currently published JAM STF and execution trace vectors, demonstrating adherence to the specification and a high level of protocol correctness.

JavaJAM has progressed beyond basic execution and now includes functional support for work package refinement, assurance generation, and auditing of work reports, covering the full lifecycle of JAM work validation. In addition, the project includes a working PVM recompiler, enabling efficient execution of JAM workloads via dynamic recompilation rather than interpretation alone.

These additional components are currently in an active phase of testing, validation, and performance verification before they will be submitted for milestone consideration.

## Deliverables

- [X] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.

| Number	| Deliverable	         | Link	 | Notes                                          |
|---------|----------------------|--------|------------------------------------------------|
|1.	      | 0.7.2 fuzzer target	 | https://github.com/methodfive/javajam/pkgs/container/javajam/605650944?tag=latest-amd64	   | |
|2.	      | JavaJAM source code	 | https://github.com/methodfive/javajam	   | Access granted on demand.                      |
|3.	      | ...	                 | ...	   | ...                                            |
|4.	      | ...	                 | ...	   | ...                                            |
|5.	      | ...	                 | ...	   | ...                                            |


## Additional Information

JavaJAM will work as-is for fuzzing with the current configuration defined in https://github.com/davxy/jam-conformance/blob/main/scripts/targets.json

If you wish to perform performance testing instead, please remove the "-Dskip.warmup=true" cmd argument.