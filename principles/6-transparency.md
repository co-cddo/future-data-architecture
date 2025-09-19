---
title: 6. Be transparent
layout: default
---
### Statement

_We are as open as possible about how our data is shared and used._

### Rationale

Transparency—observing and disclosing information about elements of and processes within a data system—is **essential for understanding if the policies and controls of the system are having the desired effect**, and why.

Transparency around actual and intended data processing operations **mitigates harm** by ensuring that risks and system failures can be detected promptly.

Clearly designating and signalling responsibilities within a data system enables responsible owners of data assets to take **meaningful accountability** for the decisions they make.

Transparency at the level of technical infrastructure means that the impact of proposed changes to the system can be understood and reasoned through, facilitating **quicker development and redress**.

Being transparent about the ways that personal data are processed and protected is a **precursor for building trust** with the public.

### Implications

**Transparency can be applied to many aspects of data sharing.** You should consider transparency measures for disclosing:

- _How and the extent to which data is processed_. Shining a light on the data flows within a data system is a vital for determining whether your system is working as intended and in the interests of its users. At a system level, insights provided by analytics dashboards and service use metrics can provide valuable, real-time information for developers and auditors of a data system. The Service Manual defines [data publishing requirements](https://www.gov.uk/service-manual/measuring-success/data-you-must-publish) for government services and the Government Analysis Function provides [guidance on creating data dashboards](https://analysisfunction.civilservice.gov.uk/policy-store/top-tips-for-designing-dashboards/).


- _The code and technical infrastructure underpinning data processing_. Coding in the open is a core tenet of the UK government’s approach to data sharing and service provision. The Technology Code of Practice requires practitioners to [be open and use open source](https://www.gov.uk/guidance/be-open-and-use-open-source), including publishing code right from the beginning of technology projects where possible. The Service Standard requires developers to [make source code open and reusable](https://www.gov.uk/service-manual/technology/making-source-code-open-and-reusable). The practice of sharing operational code is exemplified by [GDS’ code repositories](https://github.com/alphagov) on GitHub.

- _The history and provenance of data._ Providing records of a data authenticity and historical context is a crucial part of responsible data stewardship and sharing, as it allows for proper validation and audit of data. History and provenance should be captured and curated in metadata describing datasets. The Data Standards Authority describes [metadata standards for sharing and publishing data](https://www.gov.uk/government/collections/metadata-standards-for-sharing-and-publishing-data).

- _The broader context of data management_. The act of data sharing is always an enabling step in a broader data processing initiative. Data providers should clearly indicate the intended uses, responsible owners and controls around datasets to ensure downstream processing can be conducted safely and ethically. Key data management information can be captured in descriptive metadata artefacts like a Dataset Card \[link TBD\]. Where data is shared to develop or be processed by algorithmic tools and AI models, this will require reflecting in [Algorithmic Transparency](https://www.gov.uk/government/collections/algorithmic-transparency-recording-standard-hub) records.

**Transparency can and should be applied to varying extents.** It should be considered and balanced carefully against the risks of information misuse (e.g. relating to cyber security, fraud, intellectual property theft, etc.). The extent of your transparency measures should depend largely on the type and intended use of data assets within your system. You could use GDS’ guidance on [security when coding in the open](https://www.gov.uk/government/publications/open-source-guidance/security-considerations-when-coding-in-the-open) and the ICO’s guidance for [managing FOI requests](https://ico.org.uk/for-organisations/foi/guide-to-managing-an-foi-request/exemptions/) to start considering where transparency exemptions may apply within a data system.

**Transparency requires the generation and management of data about data systems**. To paint clear pictures about the activity in data systems, both automated and human initiated processes need to generate sufficient data. <span style="color:red">\[GAP: are there conventional government ways of doing this?\]</span>
