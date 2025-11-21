# JAM Milestone Delivery 

## Company/Team details

- Company/Team's name: Jampy
- Company/Team's GitHub: https://github.com/dakk
- Programming language and language set: Python (set C)
- Link/s to previous delivery/ies: -


## Documentation checklist

We declare that:

- [x] we have completed **the Web3 Foundation KYC/KYB process**.
- [x] we used **a clear and permissive open-source license**.
  - Apache License Version 2.0
- [x] we submitted **a clear Git history and public, credibly timestamped commits** | **code developed in private, with commit hashes placed, in a timely fashion, on a major public blockchain**.
  - https://polkadot.subscan.io/extrinsic?module=system&call=remark&page=1&time_dimension=date&address=12iqwZGB2sguEhjFi2ZRuWWixU8mHJnSiP1pwDefqGsBy4rV 
- [x] we used third party libraries for: **cryptographic primitives** (e.g. erasure-coding, Bandersnatch, Ed25519) | **codecs** (e.g. SCALE) | **networking** (e.g. QUIC):
  - **cryptographic primitives**: PyNaCl, ark-ec-vrfs, reed-solomon-simd, ed25519-consensus
  - **networking**: qh3, websockets
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [ ] we viewed the following **JAM implementation code** before | during our implementation.
- [x] we have not had private conversations with **other | the following implementers** regarding JAM.
- [x] we have not had **concerns about collusion**.
- [x] we agree to a recorded interview by the *Polkadot Technical Fellowship* on any matter arising from this milestone submission.
- [x] we understand that this milestone submission will need to be ratified with an on-chain remark by the *Polkadot Technical Fellowship* before it can be merged.



## Context

JamPy is an open-source implementation of the JAM protocol using the Python language, developed by Davide Gessa and released under "Apache License 2.0".

The deliverable includes a binary distribution of the target and fuzzer for graypaper version 0.7.0. The code is still not publicly available, but please contact to get access to the repo.


## Deliverables

- [x] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.


| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1.	      |M1 target and fuzzer | https://github.com/dakk/jampy-releases/tree/main/dist	   |  |
|1.	      |jampy source code | https://github.com/dakk/jampy	   | access granted on demand   |
|2.	      |...	        | ...	   |...    |
|3.	      |...	        | ...	   |...    |
|4.	      |...	        | ...	   |...    |
|5.	      |...	        | ...	   |...    |


## Additional Information

>Provide any relevant comments on the milestone submission that you would like to share with us.




