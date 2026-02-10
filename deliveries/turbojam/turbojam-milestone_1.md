# JAM Milestone Delivery 

> Don't remove any of the mandatory parts presented in bold letters or as headlines! Lines starting with >, such as this one, can be removed.


## Company/Team details

>Please provide all the required information below.

- Company/Team's name: R2 Rationality OÜ
- Company/Team's GitHub: https://github.com/r2rationality
- Programming language and language set: C++, language set B "Native code"
- Link/s to previous delivery/ies: 


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
- [x] we have not had private conversations with **other implementers**.
- [x] we have not have had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

>Please present your rationale for the completion of this milestone by connecting the deliverables and describing their purpose.

This submission is connected to the JAM Prize. The presented C++ implementation, in our opinion, adheres to all requirements for the Milestone 1 submission
and successfully passes the test vectors and public fuzzing samples for version 0.7.2 of the protocol, as published in the jam-conformance GitHub repository:
https://github.com/davxy/jam-conformance

## Deliverables

>Please indicate which **path** and **milestone** you are targeting. See [here](https://jam.web3.foundation/) for additional information.

- [x] 1. Validating Node Path
- [ ] 2. Non-PVM Validating Node Path
- [ ] 3. Light Node Path

**Milestone:** M1

>Please provide a list of all deliverables for the milestone and include links to the actual deliverables.

>Ideally all links inside the table below should include a commit hash, which will be used for testing. If you don't provide a commit hash, we will work off the default branch of your repository. Thus, if you plan on continuing work after delivery, we suggest you create a separate branch for either the delivery or your continuing work.

>If there is anything particular about any of the deliverables we or a future reader should know, use the respective Notes column.

| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1.	      |Source code | https://github.com/r2rationality/turbojam	   |    |
|2.	      |Public Docker image id the fuzzing target | r2rationality/turbojam-fuzz:latest | |
|3.       |TurboJam Configuration for the W3F Fuzzer | https://github.com/davxy/jam-conformance/blob/main/scripts/targets.json | found under "turbojam" key |


## Additional Information

>Provide any relevant comments on the milestone submission that you would like to share with us.




