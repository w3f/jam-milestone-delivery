# JAM Milestone Delivery 

## Company/Team details

- Team's name: JamBrains
- Team's GitHub: jambrains
- Programming language and language set: Elixir (set D)
- Link to previous delivery: n/a

## Documentation checklist
We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
- [x] we submitted **code developed in private, with commit hashes placed, in a timely fashion, on a major public blockchain**.
- [x] we used third party libraries for: **cryptographic primitives** (e.g. erasure-coding, Bandersnatch, Ed25519) | **networking** (e.g. QUIC) | **TLS certificate generation** | **Blake2 hashing**.
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [x] we have have had private conversations with **other implementers**.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.

## Context

We present you hereby with an implementation of the *Gray Paper v0.7.2* to claim the first milestone of the [JAM Prize](https://jam.web3.foundation/) as defined by the Web3 foundation.  
Our implementation *GrayMatter* passes all public conformance tests and is continously being improved to pass additional tests.
The repository is hosted privately on GitHub, please forward us the list of people that need access to `@oliver.tale-yazdi:parity.io` on matrix or GitHub.

Best Regards,
Kian Paimani, Francisco Aguirre and Oliver Tale-Yazdi

## Deliverables

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.

| Number | Deliverable  | Link   | Notes |
|--------|--------------|--------|-------|
|1.	     | GrayMatter   | https://github.com/JamBrains/graymatter/commits/milestone-1-rc1 | Elixir Source Code (tag `milestone-1-rc1`) |
|2.	     | Docker Image | `ghcr.io/jambrains/graymatter/gm@sha256:2cc37f1b8e0b88f47fe11b4dd717a19557331fec6457984ef4b0a1973dd9c27b` | M1 fuzzer image (sha256 `2cc37f1b8e0b88f47fe11b4dd717a19557331fec6457984ef4b0a1973dd9c27b`) |

## Additional Information

**Remarking**  
We remarked our master commit hashes to the *Polkadot Collectives* chain from the following acc 
[1jamyjYe97qPPtdeYVcUosPwc2Bv1Y6zNEMtzPW8a2z2abN](https://collectives-polkadot.subscan.io/extrinsic?address=1jamyjYe97qPPtdeYVcUosPwc2Bv1Y6zNEMtzPW8a2z2abN) in the format `{ "project": "JamBrains/graymatter", "commit": "<SHA>" }`.

**Prize Account**  
You can find our prize payout account in the RAEDME file to be `15R1pWegyu7AfMev8DBMT67qxYoJhA1v7BbA2nn7S2uJ5QDF`.
