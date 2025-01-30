# JAM Milestone Delivery 


## Company/Team details

- Company/Team's name: UNIVERSALDOT OU
- Company/Team's GitHub: https://github.com/UniversalDot
- Programming language and language set: Rust (Language set B)
- Link/s to previous delivery/ies: N/A


## Documentation checklist


We declare that:

- [x] we have completed **the Web3 Foundation KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **a clear Git history and public, credibly timestamped commits**.
- [x] we used third party libraries for: **cryptographic primitives** (e.g. erasure-coding, Bandersnatch, Ed25519) | **codecs** (e.g. SCALE) | **networking** (e.g. QUIC).
<!-- - [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation. -->
- [x] we have not had private conversations with **other implementers**.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context


This is the initial implementation of the [JAM paper](https://graypaper.com/). The current delivery includes modules for managing blocks, transactions, and smart contracts, as well as configuration settings. Each module has separated structs and logic that allows for basic creation of blockchain transactions. The current functionality covers basic state transitions and includes the basic scaffolding onto which we will build further deliverables. 


## Deliverables


- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.




| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1. License	      | MIT	        | [Link](https://github.com/UniversalDot/JAM/blob/master/LICENSE)	   |...    |
|2.	README      | Instructions for Build and Test        | [Link](https://github.com/UniversalDot/JAM/blob/master/README.md)	   |...    |
|3.	Block      |Basic implementation of Block creation        | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/src/block.rs)  |  |
|4. Blockchain	      | Blockchain implementation that is able to add transactions and check validity	        | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/src/blockchain.rs)	   |  |
|5.	Transaction      | Transactions         | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/src/transaction.rs)	   |   |
|6. Smart Contract      | Basic Function for executing Touring Complete Smart Contracts	        | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/src/smart_contract.rs)	   |    |
|7.	Utils      | Utility Functions (currently only Sha256)      | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/src/utils.rs)	   |  |
|8.	Git History      | Git History     | [Link](https://github.com/UniversalDot/JAM/commits/master/)	   |   |
|9.	Unit Tests    | Unit Test that verifies basic tests for block creating and state transitions   | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/tests/tests.rs)	   |   |


## Additional Information






