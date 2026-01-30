# JAM Milestone Delivery 

> Don't remove any of the mandatory parts presented in bold letters or as headlines! Lines starting with >, such as this one, can be removed.


## Company/Team details

>Please provide all the required information below.

- Company/Team's name: New-JAMneration
- Company/Team's GitHub: https://github.com/New-JAMneration
- Programming language and language set: Go (Set A) + Rust (Bandersnatch FFI)
- Link/s to previous delivery/ies: N/A


## Documentation checklist

>Please check the boxes to confirm that you have provided all the required documentation, providing direct links whenever possible. **DO NOT** include links to confidential or private documents.

>Chose the relevant option(s) (e.g. Option A | Option B | etc.) and delete the rest.

We declare that:

- [ ] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **a clear Git history and public, credibly timestamped commits**.
- [x] we used third party libraries for: **cryptographic primitives** ([erasure-coding](https://docs.rs/reed-solomon-simd/3.0.1/reed_solomon_simd/), [Bandersnatch](https://github.com/davxy/ark-vrf), [Ed25519](https://pkg.go.dev/filippo.io/edwards25519@v1.0.0), [Ed25519](https://pkg.go.dev/github.com/hdevalence/ed25519consensus@v0.2.0) | **networking** ([QUIC](https://github.com/quic-go/quic-go)) | **DB**([DB](https://github.com/redis/go-redis)).
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [x] we have not had private conversations with **other**.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

New-JAMneration is engineered for real-world JAM operations—correct by construction, fast under load, and resilient in production. Built in Go, it leverages a proven safety model and an ecosystem optimized for long-running services, making it a natural fit for event-driven validator and worker architectures at scale.

On correctness, the project already passes every publicly available JAM STF and execution trace test vector, providing strong evidence of specification conformance.

On functionality, it has moved beyond core execution to cover the full validation workflow: refining work packages, generating assurance, and auditing work reports. A working PVM interpreter is included for correct execution today, and a PVM recompiler is planned as a future enhancement to improve performance through dynamic recompilation.

Internal testing, validation, and performance benchmarking have been completed. The components are now ready for milestone evaluation and external verification.

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
|1.	      |	New-JAMneration source code	        | https://github.com/New-JAMneration/JAM-Protocol	   |...    |
|2.	      |...	        | ...	   |...    |
|3.	      |...	        | ...	   |...    |
|4.	      |...	        | ...	   |...    |
|5.	      |...	        | ...	   |...    |


## Additional Information

>Provide any relevant comments on the milestone submission that you would like to share with us.



