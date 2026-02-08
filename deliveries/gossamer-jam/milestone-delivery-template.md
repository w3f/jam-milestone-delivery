# JAM Milestone Delivery 

> Don't remove any of the mandatory parts presented in bold letters or as headlines! Lines starting with >, such as this one, can be removed.


## Company/Team details

>Please provide all the required information below.

- Company/Team's name: ChainSafe
- Company/Team's GitHub: https://github.com/ChainSafe
- Programming language and language set: Go (language set A)
- Link/s to previous delivery/ies: N.A


## Documentation checklist

>Please check the boxes to confirm that you have provided all the required documentation, providing direct links whenever possible. **DO NOT** include links to confidential or private documents.

>Chose the relevant option(s) (e.g. Option A | Option B | etc.) and delete the rest.

We declare that:

- [ ] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **a clear Git history and public, credibly timestamped commits**
- [x] we used third party libraries for: **cryptographic primitives** (e.g. erasure-coding, Bandersnatch, Ed25519) | **codecs** (e.g. SCALE) | **networking** (e.g. QUIC).
  - **cryptographic primitives**
    - Ed25519: [golang.org/x/crypto](https://pkg.go.dev/golang.org/x/crypto)
    - Bandersnatch [ark-vrf](https://github.com/davxy/ark-vrf)
  - **codecs**: None for M1
  - **networking**: None for M1
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
  - This is not needed for M1
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [x] we have not had private conversations with **other following implementers**.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

>Please present your rationale for the completion of this milestone by connecting the deliverables and describing their purpose.

Gossamer-JAM is a JAM node implementation in Go by ChainSafe.

The latest binary release passes all the public [test vectors](https://github.com/davxy/jam-test-vectors) and [conformance tests](https://github.com/davxy/jam-conformance) provided by the Web3 Foundation for M1.

The M1 submission targets GP 0.7.2.


## Deliverables

>Please indicate which **path** and **milestone** you are targeting. See [here](https://jam.web3.foundation/) for additional information.

- [x] 1. Validating Node Path
- [ ] 2. Non-PVM Validating Node Path
- [ ] 3. Light Node Path

- **Milestone:** M1


>Please provide a list of all deliverables for the milestone and include links to the actual deliverables.

>Ideally all links inside the table below should include a commit hash, which will be used for testing. If you don't provide a commit hash, we will work off the default branch of your repository. Thus, if you plan on continuing work after delivery, we suggest you create a separate branch for either the delivery or your continuing work.

>If there is anything particular about any of the deliverables we or a future reader should know, use the respective Notes column.

| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1.	      |Source Code	        | https://github.com/ChainSafe/go-jam	|The repository is private. Please provide the list of GitHub users that require access to @aang114 on GitHub or @aang114:matrix.org on Matrix.    |
|2.	      |Binary Releases	        | https://github.com/ChainSafe/gossamer-jam-releases	|Please use the latest release for conformance testing    |


## Additional Information

>Provide any relevant comments on the milestone submission that you would like to share with us.

N.A
