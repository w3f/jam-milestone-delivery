# JAM Milestone Delivery 

## Company/Team details

- Company/Team's name: Esscrypt / Peanut butter and JAM
- Company/Team's GitHub: https://github.com/Esscrypt
- Programming language and language set: Typescript/Assemblyscript (Set C)
- Link/s to previous delivery/ies: 
[Bandersnatch VRF](https://github.com/w3f/Grant-Milestone-Delivery/pull/1306)

## Documentation checklist

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **code developed in private, with commit hashes placed, in a timely fashion, on a major public blockchain**.
- [x] we used third party libraries for: **cryptographic primitives** (reed-solomon-simd, @noble/curves, @noble/hashes), **networking** (e.g. QUIC).
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [x] we have not had private conversations with **other | the following implementers**.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

Peanut Butter and JAM is a modular, modern TypeScript implementation of the JAM protocol, created by Mihail Kirov, designed to support Polkadot's JAM network with a focus on readability, modularity and reusability. Built with TypeScript and Bun, the project benefits from:
- TypeScript's type system: Compile-time type checking, strong IDE support, and clear interfaces reduce bugs and improve maintainability.
- Bun's performance: Fast JavaScript runtime, native bundling, and efficient package management for high-throughput validator and worker workloads.
- Modern tooling: Rich ecosystem, mature libraries, and strong developer experience for building complex protocol implementations.
- Platform independence: Cross-platform support for consistent deployment across environments.
- Event-driven architecture: Well-suited for long-running, large-scale validator and worker deployments.
The implementation has passed all currently published JAM STF and execution trace vectors, demonstrating adherence to the specification and a high level of protocol correctness.

## Deliverables

>Please check the relevant box to indicate which milestone you are delivering.

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.

| Number	| Deliverable	         | Link	 | Notes                                          |
|---------|----------------------|--------|------------------------------------------------|
|1.	      | 0.7.2 fuzzer target	 | https://github.com/Esscrypt/peanutbutterandjam	   | |
|1.	      | PBNJ source code	 | [Here](https://github.com/Esscrypt/peanutbutterandjam)	   | Access granted on demand.                      |
|3.	      | ...	                 | ...	   | ...                                            |
|4.	      | ...	                 | ...	   | ...                                            |
|5.	      | ...	                 | ...	   | ...                                            |

## Additional Information

This has been a very challenging and interesting project to work on, thank you for the opportunity to contribute.



