# JAM Milestone Delivery 

## Company/Team details

- Company/Team's name: Jam4s (https://www.jam4scala.org/)
- Company/Team's GitHub: jam4scala (https://github.com/jam4scala)
- Programming language and language set: Scala (D)
- Link/s to previous delivery/ies: N/A


## Documentation checklist


We declare that:

- [X] we have completed **the Web3 Foundation KYC/KYB process**.
- [X] we used **a clear and permissive open-source license**.
- [X] we submitted **a clear Git history and public, credibly timestamped commits** | **code developed in private, with commit hashes placed, in a timely fashion, on a major public blockchain**.
- [X] we used third party libraries for: **cryptographic primitives** (e.g. erasure-coding, Bandersnatch, Ed25519) | **codecs** (e.g. SCALE) | **networking** (e.g. QUIC).
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [X] we have had private conversations with **other implementers**.
- [X] we have not had **concerns about collusion**.
- [X] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [X] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

The Jam4s contributors initially met at Polkadot Blockchain Academy (PBA) Singapore 2024 and have been working on the JAM implementation since that time.

We hereby present our implementation of the Gray Paper **v0.7.2** to claim the first milestone of the JAM Prize, as defined by the Web3 Foundation.

The Jam4s implementation successfully passes all public conformance tests. The implementation is actively maintained to remain compatible with newly released test vectors and includes support for the updated gas model.

The main repository is currently hosted privately on GitHub. Access can be requested via Matrix from:
- `@celadari:matrix.org` (Charles-Edouard LADARI)
- `@subotic:matrix.org` (Ivan SUBOTIC)
- `@basedaf_dev:matrix.org` (Thomas LIU)
- `@sergei_astapov:matrix.org` (Sergei ASTAPOV)

## Deliverables

- [X] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.


| Number | Deliverable | Link | Notes                                       |
|------:|------------|------|---------------------------------------------|
| 1 | Jam4s core implementation (Importer) | https://github.com/jam4scala/jam4s | Private repository – access available upon request |
| 2 | Jam4s Docker image | `jamforscala/jam4s:0.7.2-rc.9-amd64` | Prebuilt image for reproducible testing     |
| 3 | Jam4s Crypto JNA source | https://github.com/jam4scala/jam4s-crypto-jna | Java ↔ Rust crypto bindings (linux-amd64, darwin, windows) |
| 4 | Jam4s Crypto JNA Maven artifact | https://central.sonatype.com/artifact/org.jam4s/jam4s-crypto-jna | Published library                           |
| 5 | Jam4s codec source | https://github.com/jam4scala/jam4s-codec | codec implementation |
| 6 | Jam4s codec (core) Maven artifact | https://central.sonatype.com/artifact/org.jam4s/jam4s-codec-core_3 | Published library                           |
| 7 | Jam4s codec CLI Maven artifact | https://central.sonatype.com/artifact/org.jam4s/jam4s-codec-cli_3 | CLI tooling                                 |
| 8 | Jam4s external test vectors repo | https://github.com/jam4scala/jam4s-external | Test vectors and parsing logic kept separate from core repo |



## Additional Information

- The implementation passes all JAM conformance tests for Gray Paper v0.7.2, as reported in the `jam-conformance` repository:
  https://github.com/davxy/jam-conformance/blob/main/fuzz-reports/0.7.2/summaries/summary_jam4s.txt
- Test vectors are intentionally stored in a separate repository to avoid bloating the main Jam4s codebase.
- The implementation is continuously updated to track new conformance tests and specification changes.
- Performance benchmarking and authoring functionality are planned for subsequent milestones.

