# JAM Milestone Delivery 
## Company/Team details
- Company/Team's name: JAMdot Technologies VOF
- Company/Team's GitHub: https://github.com/JAMdotTech
- Programming language and language set: Python (Set C)
- Link/s to previous delivery/ies: Not Applicable

## Documentation checklist
We declare that:
- [X] we have completed **the Web3 Foundation KYC/KYB process**.
- [X] we used **a clear and permissive open-source license**.
- [X] we submitted **a clear Git history and public, credibly timestamped commits**.
- [X] we used third party libraries for: **cryptographic primitives** (`py-bandersnatch-vrfs`, `py-ed25519-zebra`, `pycryptodome`) | **networking** (`aioquic`).
- [ ] we provided **Gas, trie/DB, signature-verification, and availability (EC/DB) performance tests** to be run on standard hardware.
- [X] we have not viewed **JAM implementation code** before or during our implementation.
- [X] we have not had private conversations with **other implementers**.
- [X] we have not had **concerns about collusion**.
- [X] we agree to a recorded interview by the **Polkadot Technical Fellowship** on any matter arising from this milestone submission.
- [X] we understand that this milestone submission will need to be ratified with an on-chain remark by the **Polkadot Technical Fellowship** before it can be merged.

## Context
This document covers Milestone 1 Delivery for PyJAMaz - a Python Implementation of JAM protocol by the Netherlands-based company JAMdot Technologies.

In June 2024, Arjan and Emiel begin exploring a Python implementation of the JAM Protocol under the name PyJAMaz. In the period leading up to September 2024, a rudimentary prototype of PyJAMaz is developed by Arjan and Emiel. During this period, Matthijs is recruited to strengthen the team. This results in a complementary skill set within the team with a clear division of responsibilities: Emiel possesses broad knowledge of the Gray Paper and the Polkadot architecture, Arjan assumes the role of application architect, and Matthijs contributes his specialized expertise in virtual machines and performance fine-tuning. There is confidence that Arjan and Matthijs together possess more than sufficient Python expertise to develop the fastest possible Python implementation of the JAM Protocol. On September 1 2024, Matthijs fully joins the research and development team, and in October Peter strengthens the team by providing organizational support. The team formulates the objective of working toward achieving JAM Prize Milestones 1 and 2 within a period of approximately 24 months, which entails full conformance with the Gray Paper.

## Deliverables
- [X] 1. IMPORTER: State-transitioning conformance tests pass and can import blocks.

| Number	| Deliverable	| Link	 | Notes |
|---------|-------------|--------|-------|
|1.	      |v0.7.2 M1 Fuzzer Target |[Docker Hub](https://hub.docker.com/r/jamdottech/pyjamaz) | Tag: `v0.1.45-gp0.7.2` or `latest`; [JAM Conformance Repository](https://github.com/davxy/jam-conformance/blob/main/scripts/targets.json)  |
|2.	      |v0.7.2 M1 Source Code |[GitHub](https://github.com/JAMdotTech/pyjamaz) |Web3 Foundation or Fellowship reviewers can be granted access on request |

## Additional Information
### Research & Development Journal 2024–2025
#### Functional Conformance Milestone 1 (July 2024 – March 2025)

The team’s first priority is achieving Milestone 1 of the JAM Prize. Broadly speaking, this involves implementing a node application with the objective of importing a blockchain data structure of a JAM network. This phase of the project is divided into two parallel tracks:

1. Arjan, with support from Emiel, is responsible for implementing Chapters 3 through 13 and Appendices C through H (excluding Appendix G) of the Gray Paper. This concerns the implementation of the runtime with the state transition function (STF) of the JAM Protocol.

2. Matthijs, with support from Emiel, is responsible for implementing Appendix A and part of Appendix B of the Gray Paper. This concerns the implementation of the PVM (Polkadot Virtual Machine) and the host functions through which this execution environment can be embedded in the JAM Protocol.

Up to February 2025, the above activities take place in parallel. Thereafter, the team works together to merge the two separate components into a coherent whole, resulting in functional conformance with Milestone 1 for Gray Paper v0.6.2 in March 2025.

#### Release Cycles Conformance Milestone 1 (March 2025 – December 2025)

Following the achievement of functional conformance for Milestone 1, a regular release cycle is adopted for PyJAMaz. During this period, the Gray Paper is regularly updated with functional refinements to the JAM Protocol. The release cycle of the Python implementation aims to maintain functional conformance with the Milestone 1 objectives in response to these changes. A systematic iteration through successive versions of Gray Paper 0.6.3 through 0.6.7 takes place by following the official Web3 Foundation conformance test vectors.

During the JAM Experience Implementers Meetup in Lisbon in May 2025, cautious indications are given that the audit process may commence from September 2025 onward for teams claiming Gray Paper conformance for Milestone 1.

#### Informal Conformance Audit Milestone 1 (August 2025 – December 2025)

From August 2025 onward, the various independent implementation teams may indicate that their respective implementations are ready to participate in the conformance audit. The team begins its participation in this process as the 9th team on August 19, 2025. This activity entails that the various implementations must additionally support the Fuzzer Protocol so that Web3 Foundation can ultimately demonstrate Milestone 1 conformance in a uniform manner. These fuzzer activities enable Web3 Foundation to apply random sequences of state transitions to the various implementations.

The primary objective of the fuzzer activities is to identify disputes between the different independent implementations of the JAM Protocol. Finding disputes does not necessarily imply that an implementation has correctly or incorrectly implemented the JAM Protocol specification, but rather that there are differing interpretations of the Gray Paper. Teams are encouraged to engage in mutual discussions regarding these disputes in order to eliminate any possible ambiguity in the Gray Paper. A concrete side effect of this fuzzer process is the observation that a large number of disputes exist, leading to the conclusion that no team has yet achieved the intended conformance for Milestone 1. Teams are encouraged to continue working toward conformance within the cleanroom rules applicable to the JAM Prize. Suggestions are made to independently pursue additional quality activities to achieve conformance, such as close-reading sessions of the Gray Paper, developing documentation, developing additional test vectors, independently developing a fuzzer protocol, independently developing a JAM Service SDK, and so forth.

In addition to the conformance criteria for the JAM Prize, it becomes clear that performance criteria will also apply to the JAM Prize (for Milestone 1). These additional criteria initially come as a surprise to the team (and to many other teams as well), as it had been assumed that performance-related criteria for JAM implementations would only become relevant during Milestones 3 and 4. The reasons for these performance criteria relate to the manner in which conformance for Milestone 1 must be demonstrated. The JAM Protocol described in the Gray Paper constitutes a formal specification, and each individual implementation must prove that it is fully conformant with this specification. Through a battery of traces (i.e., scenarios) using the Fuzzer Protocol developed by Web3 Foundation, this conformance will be demonstrated. The ideal objective is to test all theoretical logical paths of the JAM Protocol implementations without disputes arising between the different implementations. Each implementation must pass a large (but inherently finite) set of traces in order to achieve, on the basis of equality, an objectively high level of confidence in conformance.

Initial benchmarks of the implementations by the various teams reveal very large performance variance during fuzzer activities. Some implementations are more than a factor of 100 slower than the fastest ones. The argument is that if the conformance audit for the fastest implementations yields the desired confidence level over a test period of three days, the audit process for slower implementations could take more than a year. This extremely long audit duration is undesirable, and implementation teams are encouraged to apply performance optimizations, both in their own interest and in the interest of efficient resource allocation by the audit team.

Between August 2025 and October 2025, significant performance improvements are implemented in PyJAMaz, resulting in a 93% reduction in benchmark execution time. Although PyJAMaz is a Python implementation of the JAM Protocol and therefore can never inherently reach the same performance range as a Rust or C++ implementation, these improvements make the Python implementation the fastest in its class and place it within a team-defined acceptable range of less than a factor of 20 slower than the fastest implementation in the comparative benchmark. As a result, the expected duration of the formal conformance audit for Milestone 1 is reduced to a maximum of two months.

During this phase, Web3 Foundation provides a standardized set of tests. These make disputes between implementations visible and indirectly demonstrate conformance (either through consensus or through the absence of disputes between implementations). These tests are expanded with various groups targeting specific functionality and specific edge cases. In November 2025, the intended audit team indicates that sufficient confidence is beginning to emerge that the first implementations are ready for the Milestone 1 conformance audit. At the end of November 2025, it is therefore announced that during December 2025 the developed audit process will be transferred to a dedicated Web3 Foundation team. This new audit team is expected (subject to confirmation) to commence the formal Milestone 1 conformance audit in January 2026. In retrospect, the period from August 2025 through December 2025 can thus be regarded as the informal Milestone 1 conformance audit. The team expects its implementation, PyJAMaz, to be among the first teams to participate in the formal Milestone 1 audit process.

#### Functional Conformance Milestone 2 (from October 2024)

Although the team’s primary priority is achieving Milestone 1 of the JAM Prize, work on functional conformance for Milestone 2 proceeds in parallel. In particular, during periods when waiting times arise for Milestone 1 activities, time is productively spent on Milestone 2 tasks. This milestone broadly involves implementing a node application capable of functioning as a full block producer. This includes implementing Chapters 14 through 19 and part of Appendix B, as well as the entirety of Appendix G, of the Gray Paper.

#### Other Activities

In addition to the milestone-related research and development activities, the team has contributed to the creation and audit of the formal specification of the JAM Protocol by providing contributions to the Gray Paper.

The team has organized activities for and actively participated in various meetings for coordination and collegial discussion (within cleanroom rules).

During the last quarter of 2025, exploratory work was conducted toward the development of a so-called PVM SDK for Python. Such an SDK (software development kit) provides opportunities to write software in a subset of the Python programming language that can be executed by the PVM execution environment. Possible applications of this SDK include the development of JAM Services with Refine and Accumulate entry points or PVM smart contracts (initially for Kusama and Polkadot AssetHub).

#### Summary of Activities
Milestone 1
- March 2025: Milestone 1 Conformance Gray Paper v0.6.2, Official Web3 Foundation Conformance Test Vectors
- July 2025: Milestone 1 Conformance Gray Paper v0.6.6
- August 2025: Milestone 1 Conformance Gray Paper v0.6.7, Start Informal M1 Conformance Audit
- September 2025: Fuzzer (Target) Protocol, Start Performance Improvements PyJAMaz
- October 2025: Milestone 1 Conformance Gray Paper v0.7.0
- November 2025: Milestone 1 Conformance Gray Paper v0.7.1
- December 2025: Milestone 1 Conformance Gray Paper v0.7.2, Announcement Formal W3F M1 Conformance Audit

Event Attendance
- June 2024: Brussels JAM Lecture
- October 2024: Lisbon JAM Meetup
- November 2024: Bangkok JAM Meetup
- May 2025: Lisbon JAM Meetup

Other
- 2024–2025: Contributions to Gray Paper Audit
- 2024-2025: Miscellaneous Milestone 2 Work
- November 2025: JAM Service SDK MVP
