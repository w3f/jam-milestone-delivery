# JAM Milestone Delivery 

> Don't remove any of the mandatory parts presented in bold letters or as headlines! Lines starting with >, such as this one, can be removed.


## Company/Team details

>Please provide all the required information below.

- Company/Team's name: UNIVERSALDOT OU
- Company/Team's GitHub: https://github.com/UniversalDot
- Programming language and language set: Rust (Language set B)
- Link/s to previous delivery/ies: N/A


## Documentation checklist

>Please check the boxes to confirm that you have provided all the required documentation, providing direct links whenever possible. **DO NOT** include links to confidential or private documents.

>Chose the relevant option(s) (e.g. Option A | Option B | etc.) and delete the rest.

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **a clear Git history and public, credibly timestamped commits** | **code developed in private, with commit hashes placed, in a timely fashion, on a major public blockchain**.
- [x] we used third party libraries for: **cryptographic primitives** (e.g. erasure-coding, Bandersnatch, Ed25519) | **codecs** (e.g. SCALE) | **networking** (e.g. QUIC).
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [ ] we have not | have had private conversations with **other | the following implementers**.
- [ ] we have not | have had **concerns about collusion**.
- [ ] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [ ] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

>Please present your rationale for the completion of this milestone by connecting the deliverables and describing their purpose.


## Deliverables

>Please check the relevant box to indicate which milestone you are delivering.

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.


>Please provide a list of all deliverables for the milestone and include links to the actual deliverables.

>Ideally all links inside the table below should include a commit hash, which will be used for testing. If you don't provide a commit hash, we will work off the default branch of your repository. Thus, if you plan on continuing work after delivery, we suggest you create a separate branch for either the delivery or your continuing work.

>If there is anything particular about any of the deliverables we or a future reader should know, use the respective Notes column.

| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1. License	      | MIT	        | [Link](https://github.com/UniversalDot/JAM/blob/master/LICENSE)	   |...    |
|2.	README      | Instructions for Build and Test        | [Link](https://github.com/UniversalDot/JAM/blob/master/README.md)	   |...    |
|3.	Block      |Basic implementation of Block creation        | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/src/block.rs)  | [Tests](https://github.com/UniversalDot/JAM/blob/master/jam/tests/block.rs)   |
|4. Blockchain	      | Blockchain implementation that is able to add transactions and check validity	        | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/src/blockchain.rs)	   |[Tests](https://github.com/UniversalDot/JAM/blob/master/jam/tests/blockchain.rs)   |
|5.	Transaction      | Transaction Struct        | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/src/transaction.rs)	   | [Tests](https://github.com/UniversalDot/JAM/blob/master/jam/tests/transaction.rs)   |
|6. Smart Contract      | Basic Function for executing Touring Complete Smart Contracts	        | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/src/smart_contract.rs)	   | [Tests](https://github.com/UniversalDot/JAM/blob/master/jam/tests/smart_contract.rs)    |
|7.	Utils      | Utility Functions (currently only Sha256)      | [Link](https://github.com/UniversalDot/JAM/blob/master/jam/src/utils.rs)	   |[Tests](https://github.com/UniversalDot/JAM/blob/master/jam/tests/utils.rs)   |


## Additional Information

>Provide any relevant comments on the milestone submission that you would like to share with us.




