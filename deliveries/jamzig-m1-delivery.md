# JAM Milestone Delivery 

## Company/Team details

- Company/Team's name: JamZig⚡ https://jamzig.dev/
- Company/Team's GitHub: https://github.com/jamzig
- Programming language and language set: Zig 
- Link/s to previous delivery/ies: None

## Documentation checklist

We declare that:

- [X] we have completed **the Web3 Foundation KYC/KYB process**.
- [X] we used **a clear and permissive open-source license**.
- [X] we submitted **a clear Git history and public, credibly timestamped commits**.
- [X] we used third party libraries for: **cryptographic primitives** (e.g. erasure-coding, Bandersnatch, Ed25519): https://github.com/jamzig/jamzig/tree/main/ffi/rust/crypto
- [X] we used third party libraries for  **networking** (e.g. QUIC) https://github.com/jamzig/lsquic#ee141c51f1257718c639edf78e300724b38dcb46.
- [X] we provided **no** performance tests to be run on standard hardware.
- [X] we viewed the **no** implemenation code before or during our implementation.
- [X] we have not  had private conversations with **other implementers** on the subject of JAM code.
- [X] we have not had **concerns about collusion**.
- [X] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [X] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.


## Context

This represents our JamZig M1 delivery, completed as a solo
implementation effort. For deeper insights into our journey and project
evolution, check out our X profile at https://x.com/jamzig_dev. 

The codebase and executable we're submitting has been "refined" to deliver
precisely what M1 demands—nothing more, nothing less. Behind the scenes, I'm
actively developing networking capabilities and developer tooling in a private
repository, laying the groundwork for what's next. This work is boosted by the
co-founded Polana project (https://polana.network), where we've successfully
ported the SVM into a JAM service running on our JamZig implementation which is
capable of running sBPF Solana contracts. 

Additionally, Akasha Void
(https://akashavoid.io), a soon-to-be-released space trader game, is being
prototyped to run on JAM's continuous execution framework. 

You can follow Polana's progress at https://x.com/polana_network. 

## Deliverables

- [X] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.


| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1.	      |M1	          | https://github.com/jamzig/conformance-releases  | M1 v0.7.2 Fuzz Target    |
|2.	      |...	        | ...	   |...    |
|3.	      |...	        | ...	   |...    |
|4.	      |...	        | ...	   |...    |
|5.	      |...	        | ...	   |...    |


## Project Timeline

**Development:** Aug 2024 - Dec 2025 (16 months, ~2,000 commits, solo)

**Phase 1 - Foundation (Aug-Sep 2024):** 171 commits
- Aug 22: Initial commit
- Aug 27: Test vector infrastructure
- Aug 30: Rust FFI integration (Bandersnatch VRFs)
- Sep 4-8: Safrole consensus, entropy module, state transitions

**Phase 2 - Core Protocol (Oct 2024 - Apr 2025):** 905 commits
- Accumulation, assurances, ordered accumulation
- Network threads, JAM fetch
- State roundtrip testing

**Phase 3 - Advanced Features (May-Jul 2025):** 520 commits
- Jun (peak): 278 commits
- Jul: Fuzzing protocol, traces, refactoring (Merkle, accumulation, authorizer pool)

**Phase 4 - v0.7.0 Migration (Aug-Sep 2025):** 331 commits
- Tracy profiler integration
- PVM optimizations: flat memory O(1) access, binary search, non-recursive, parallel header validation
- Fuzz protocol v1, fork detection, state ancestry tracking

**Phase 5 - v0.7.1 Compliance (Nov-Dec 2025):** 53 commits
- Nov 20: v0.7.0 complete
- Nov 28: v0.7.1 compliance (service stats, chi privileges, accumulation fixes)
- Dec 14: v0.7.1 conformance (iteration ordering, preimage validation, theta sorting)

**Phase 6 - v0.7.2 (Dec 2025):** Current release

**Releases:**
v0.6.5 (May 2025) → v0.6.6 (Jul) → v0.6.7 (Aug) → v0.7.0 (Nov) → v0.7.1 (Nov 28) → v0.7.2 (Dec)

**Event Attendance:**
- Bangkok JAM Meetup (Nov 2024)
- Lisbon JAM Meetup (May 2025)

## Additional Information

First of all, it is a privilege to be part of this unique event in history!

I reached all M1 importer requirements months ago and have been iterating to
stay current with the latest protocol (graypaper) changes. This submission is a
placeholder for the actual submission, to make sure we have dotted all the i's
and completed KYC. The link to the executable will be provided once the fuzzing
protocol has been shared and I have built a release that can be fuzzed.

Achieving graypaper conformance proved revelatory—precision at the bit-and-byte
level demands rigorous discipline. While challenging, this exactitude is
foundational to JAM's decentralization: only through multiple independent,
specification-perfect implementations can the protocol achieve the resilience
and trust-minimization it promises.

I have read and hereby sign the JAM Prize Terms and Conditions.
