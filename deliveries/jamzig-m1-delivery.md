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

You can follow Polana's progress at https://x.com/polana_network. 

## Deliverables

- [X] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.
- [ ] 2. AUTHOR: Fully conformant and can produce blocks (including networking, off-chain).
- [ ] 3. HALF-SPEED: Conformance and Kusama-level performance (including PVM implementation).
- [ ] 4. FULL-SPEED: Conformance and Polkadot-level performance (including PVM implementation).
- [ ] 5. SECURE: Fully audited.


| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1.	      |M1	          | https://github.com/jamzig/conformance-releases/tree/main/releases/202507062117_3616ff7	   | M1 v0.6.6 Fuzz Target    |
|2.	      |...	        | ...	   |...    |
|3.	      |...	        | ...	   |...    |
|4.	      |...	        | ...	   |...    |
|5.	      |...	        | ...	   |...    |


## Additional Information

First of all, it is a privilege to be part of this unique event in history!

I reached all M1 importer requirements months ago and have been iterating to
stay current with the latest protocol (graypaper) changes. This submission is a
placeholder for the actual submission, to make sure we have dotted all the i’s
and completed KYC. The link to the executable will be provided once the fuzzing
protocol has been shared and I have built a release that can be fuzzed.

I have read and hereby sign the JAM Prize Terms and Conditions.

