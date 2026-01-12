# JAM Milestone Delivery 

## Company/Team details

- Company/Team's name: FastRoll
- Company/Team's GitHub: https://github.com/fastroll-jam
- Programming language and language set: Rust (language set B)
- Link/s to previous delivery/ies: None


## Documentation checklist

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **code developed in private, with commit hashes placed, in a timely fashion, on a major public blockchain**.
- [x] we used third party libraries (rust crates) for:
    - **cryptographic primitives**: ark-vrf (Bandersnatch), blake2 (Blake2b), ed25519-consensus (Ed25519), reed-solomon-simd (erasure-coding), sha3
    - **codecs**: SCALE (modified Parity version to implement JAM codec), base32, hex
    - **networking**: quinn (QUIC), rcgen, rustls
    - **database**: rocksdb
    - **async runtime**: tokio
    - **utilities**: dashmap, mini-moka, rayon, bitvec, clap, and others defined in Cargo.toml
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [x] we have not had private conversations with **other implementers**.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

- FastRoll is a Rust implementation of JAM developed independently by Junha Park since July 2024.
- This delivery covers Milestone 1, focusing on state transition conformance and block import functionalities.
- The implementation is strictly based on Graypaper, currently targeting v0.7.2. During development, I contributed PRs to the Graypaper repository to fix errors and typos discovered in the spec.
- The binary supports a fuzz target runner, passes all public test vectors (STF and block traces), and is participating in fuzzing: https://github.com/davxy/jam-conformance/issues/45
- I have prioritized idiomatic Rust and clean architecture. As this is the importer milestone, post-M1 systems like networking are currently in early stages. Future milestones will focus on the "validating node path", including PVM recompiler and performance optimization.


## Deliverables

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.


| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1.	      |FastRoll Source Code|https://github.com/fastroll-jam/fastroll	   |Currently Private Repo|
|2.	      |Binary Releases|https://github.com/fastroll-jam/fastroll-releases/releases	   |For conformance testing|
|3.	      |Public Commit Hashes|https://etherscan.io/advanced-filter?fadd=0x25BA43364BF720d8dFe3c2680CB4C232a29B093C&tadd=0x25BA43364BF720d8dFe3c2680CB4C232a29B093C&txntype=0&qt=1	   |Used Ethereum to snapshot commit hashes|


## Additional Information

- FastRoll source code is private. I will make it public once the official auditing begins, or grant access to auditors/reviewers upon request.
