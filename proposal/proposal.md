## Title: SoK: Hardware-Assisted Control-Flow-Integrity

## Introduction

Control flow hijacking is an attack where the attacker diverts the control flow of the program from its intended path to malicious code, and it remains a prevalent vulnerability. According to Common Vulnerabilities and Exposures Project [CVE], tens of control flow hijacking vulnerabilities have been reported since 2025, allowing attackers to leak confidential information, escalating privilege, or executing arbitrary code. As a mitigation, Control Flow Integrity (CFI) is a group of security mechanisms that ensures the control flow follows a predetermined path of a Control Flow Graph [Abadi].

CFI can be implemented by software-based measures, hardware-based measures, or hardware-assisted measures. Hardware-assisted CFI leverages both hardware and software defense, so it is also referred to as a hybrid approach. Pure hardware-based and software-based approaches have been criticized for high performance overhead and long time-to-market [Kumar 2022]. Therefore, the number of hardware-assisted CFI has been growing rapidly in recent years. Efforts have been made to systematically review and evaluate them, and to the best of my knowledge, the most recent systematic review was published in 2022 [Kumar 2022]. However, giving the fast-moving nature of this field and the number of new methods proposed, a new systematic review is required to address the gap to provide insights into recent developments of CFI.

## Research Questions

This research aims to answer the following research questions:

- RQ1: What hardware-assisted CFI are proposed from 2022?
- RQ2: How effective are they against new control flow hijacking attacks?
- RQ3: Whare are the tradeoffs made by them in terms of feasibility and performance overhead?
- RQ4: What open problems are to be addressed in this field?

## Methodology

I will follow the Preferred Reporting Items for Systematic reviews and Meta-Analyses (PRISMA) framework [Page 2021], which sets out the guidelines for systematic review methodology. In addition, I will adopt the PRISMA Checklist [PRISMA CheckList] items to the need of this SoK paper, as outlined in this section.

### Eligibility Criteria

After the initial searching phase is completed, I will assess the appropriateness of studies using the following eligibility criterias:

- EC1: The study must directly address the field of computer memory security in the context of CFI.
- EC2: The study must either a. propose a CFI mechanism or b. review a CFI mechanism.
- EC3: The CFI addressed in the study must be hardware-assisted. That is, it must be a hybrid method that is implemented on both hardware and software level.
- EC4: The study must be published in or after 2022.
- EC5: The study must be absent from the list of CFI evaluated in [Kumar22].

### Information Sources

Sources will be primarily selected from digital libraries including ACM Digital Library [ACM DLIB], IEEE Xplore [IEEE Xplore], arXiv [arXiv], MDPI [mdpi], Springer Nature Link [Springer], and ScienceDirect [ScienceDirect] and security publication venues including USENIX [USENIX] and NDSS [ndss]. I will also use Google Scholar [GoogleScholar] for forward and backward citation chasing.

### Search Strategy

I will first use a combination of keywords decided by me, and add more keywords that occur frequently in the papers I collected. After the initial pass of collecting and screening sources, I will proceed to use forward and backward citation chasing to collect more related work. Subsequently, I will remove all duplicate items and assess newly added sources against the eligibility criterias.

The search results are expected to be exported in August 2026.

### Synthesis Method

By tabulating the CFI characteristics and comparing them against the defense evaluated in [Kumar 2022], I will map all sources to the taxonomy proposed by Kumar et al., which categorizes hardware-assisted CFI into binary-based defense, process-based defense, and system-based defense. If a defense does not fit into these three categories, I will evaluate it separtely and try to aggregate such outlying defenses in case a new type of CFI occured after 2022.

After mapping the defenses, I will extract the common characteristics within the aforementioned subgroups and try to identify any open problems.

## Expected Outcome

I expected the study to extend the taxonomy developed by [Kumar 2022] by systematically classifying recent hardware-assisted CFI. In addition, the study will, upon its successful completion, provide a comparative analysis of groups of CFI in terms of implementation feasibility, performance overhead, and to what extent they mitigate control flow hijacking. Finally, it will highlight the open questions that need to be addressed in future research.

## Plan B

If I fail to identify a research gap to focus on, or if no orignial insights can be extracted, I will instead change this paper into a replication and extension of [Kumar 2022].

## References