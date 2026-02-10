# JAM Milestone Delivery 

> Don't remove any of the mandatory parts presented in bold letters or as headlines! Lines starting with >, such as this one, can be removed.


## Company/Team details

>Please provide all the required information below.

- Company/Team's name: Laminar
- Company/Team's GitHub: https://github.com/open-web3-stack
- Programming language and language set: B
- Link/s to previous delivery/ies: N/A


## Documentation checklist

>Please check the boxes to confirm that you have provided all the required documentation, providing direct links whenever possible. **DO NOT** include links to confidential or private documents.

>Chose the relevant option(s) (e.g. Option A | Option B | etc.) and delete the rest.

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **a clear Git history and public, credibly timestamped commits**.
- [x] we used third party libraries for: **cryptographic primitives** (e.g. erasure-coding, Bandersnatch, Ed25519) | **networking** (e.g. QUIC).
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [x] we have not had private conversations with **other | the following implementers**.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

>Please present your rationale for the completion of this milestone by connecting the deliverables and describing their purpose.

Boka implements the fuzz-protocol defined at [jam-conformance](https://github.com/davxy/jam-conformance) and have passed all the public tests includeing [jamtestvectors](https://github.com/w3f/jamtestvectors).

A public docker image is provided the node. Otherwise the readme provides the instructions to build the node from source.

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
|1.	      | Code | https://github.com/open-web3-stack/boka	   |    |
|2.	      | Docker Image	        | https://hub.docker.com/r/acala/boka	   |    |


## Additional Information

>Provide any relevant comments on the milestone submission that you would like to share with us.




