## Introduction
    ### Relevance of Control Flow Hijacking
        - CVE -> How prevalent it is
    ### Landscape of Defenses
        - Main categories of defenses, software-based, hardware-based, and hardware-assisted
    ### Definition of Hardware-Assisted CFI
    ### RQs
        - RQ1: What hardware-assisted CFI are proposed from 2022?
        - RQ2: How effective are they against new control flow hijacking attacks?
        - RQ3: What are the tradeoffs made by them in terms of feasibility and performance overhead?
        - RQ4: What open problems are to be addressed in this field?
## Background
    ### Control Flow Hijacking Attacks (How do they work)
        - Major categories of attacks, e.g., return-oriented programming, data-oriented programming, etc.
    ### Previous Work
        - What previous systematic review exist
        - Why is a new SoK needed
## Methodology
    ### Search Strategy
        - Query per Database (Query string for ACM Digital Library, IEEE Xplore, arXiv, ...)
    ### Selection Criteria
        - EC1: The study must directly address the field of computer memory security in the context of CFI.
        - EC2: The study must either 1. propose a novel CFI defense or 2. evaluate a CFI defense.
        - EC3: The CFI addressed in the study must be hardware-assisted. That is, it must be a hybrid method that is implemented on both hardware and software levels.
        - EC4: The study must be published in or after 2022 and not reviewed already in the Kumar 2022 paper.
    ### Taxonomy
        - Binary-based, Process-based, and system-based taxonomy proposed by Kumar et al.
        - Explain why this specific taxonomy is used over all others
## Results of the Search and Selection Process
    ### Summary Statistics with Flowchart (How many papers remain at each stage)
    ### Explain why some studies that appear to meet the criteria are excluded
    ### A Table of Defenses Used in Each Paper
        - e.g., Binary rewriting, shadow stack, branch verification, etc.
## Hardware-Assisted CFI
    ### Binary-Based
    ### Process-Based
    ### System-Based
## Discussion
    ### Comparing effectiveness / implementation cost
    ### Development of mitigations from 2022 (Trends)
    ### Limitations
        - Limitation of inclusion & exclusion criteria
        - Limitation of taxonomy (if applicable)
## Conclusion
    ### Future Outlooks
    ### Contribution