# JAM Milestone Delivery

## Company/Team details

- Company/Team's name: Jamzilla
- Company/Team's GitHub: https://github.com/ascrivener
- Programming language and language set: Go (A)
- Link/s to previous delivery/ies: N/A


## Documentation checklist

I declare that:

- [x] I have completed **the Web3 Foundation KYC/KYB process**.
- [x] I used **a clear and permissive open-source license**.
- [x] I submitted **a clear Git history and public, credibly timestamped commits**
- [x] I used third party libraries for: **cryptographic primitives** (Bandersnatch, Ed25519) and **networking** (QUIC).
- [N/A] I provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [x] I viewed NO **JAM implementation code** before OR during my implementation.
- [x] I have not had private conversations with **any implementers**.
- [x] I have not had **concerns about collusion**.
- [x] I agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] I understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

Jamzilla is a JAM protocol implementation written in Go with Rust cryptographic primitives.

The jamzilla-tiny binary deliverable passes all state-transitioning conformance tests from the official jam-conformance test vectors, demonstrating correct implementation of the JAM protocol's import functionality.


## Deliverables

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.

| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1.	      |jamzilla binary (tiny)	        | https://github.com/ascrivener/jam/tree/main	   |Build with `./build.sh`. Run with `./bin/jamzilla-tiny`.    |


## Additional Information

The deliverables in this milestone target GP 0.7.2. The main branch of the repository will target GP 0.7.2 for the duration of submission evaluation.

To verify conformance tests:
```bash
./build.sh
./bin/jamzilla-tiny &
cd src/go && go test ./cmd/fuzzer/fuzzclient -run TestConformanceVectors -v
```

This milestone implements the IMPORTER requirements: state-transitioning conformance tests pass and blocks can be imported.




