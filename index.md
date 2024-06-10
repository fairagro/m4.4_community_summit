- **Antonia Leidel**<sup>1</sup> [![E-Mail](./assets/mail.svg)](mailto:leidel@ipk-gatersleben.de)
- **Dr. Jens Krumsieck**<sup>2</sup> [![ORCID: 0000-0001-6242-5846](./assets/orcid.png)](https://orcid.org/0000-0001-6242-5846) [![E-Mail](./assets/mail.svg)](mailto:jens.krumsieck@thuenen.de)
- **Patrick König**<sup>1</sup> [![ORCID: 0000-0002-8948-6793](./assets/orcid.png)](https://orcid.org/0000-0002-8948-6793) [![E-Mail](./assets/mail.svg)](mailto:koenig@ipk-gatersleben.de)
- **Dr. Harald von Waldow**<sup>2</sup> [![ORCID: 0000-0003-4800-2833](./assets/orcid.png)](https://orcid.org/0000-0003-4800-2833) [![E-Mail](./assets/mail.svg)](mailto:harald.vonwaldow@thuenen.de)
- **Florian Hoedt**<sup>2</sup>[![ORCID: 0000-0002-6068-1659](./assets//orcid.png)](https://orcid.org/0000-0002-6068-1659) [![E-Mail](./assets/mail.svg)](mailto:florian.hoedt@thuenen.de)

on behalf of the FAIRagro consortium

<sup>1</sup> Leibniz Institute of Plant Genetics and Crop Plant Research, IPK - 
<sup>2</sup> Thünen Institute

## Abstract

FAIR[^1] research is becoming increasingly important, but developing and publishing FAIR computational workflows can be challenging. A Scientific Workflow Infrastructure (SciWIn) will support scientists during data exploration and analysis with version control, the recording of workflows and provenance tracking. Specific tooling will help to formally specify annotated workflows, making them executable on different workflow engines. SciWIn will also facilitate collaboration and let researchers share, re-use, combine and extend workflows and associated data and code. The state-of-art annotation with metadata and encapsulation in FAIR Digital Objects (FDOs) will foster the FAIR publication of high-quality scientific work and help to further establish Open Science practices.
 
## Concept
![Concept](./assets/SciWInRO.svg)
![Concept](./assets/SciWInConcept.svg)

As this is an early concept of SciWIn, details may change in the future, but the overall idea is presented herein. Implied by the name "Scientific Workflow Infrastructure" (SciWIn) the **execution of computational workflows** will be a key feature of SciWIn. Researchers will be able to interact with the easy-to-use interface of **SciWIn Hub** by using some kind of **SciWIn Client Software** to work on and create new research objects (RO) containing new or already existing computational workflows. Research objects will be sent as RO-Crates.

When handled by SciWIn Hub, an RO will get a PID[^3] (e.g. DOI[^4]) since ROs will be represented as FAIR DOs[^5] (FDO) on SciWIn Hub. 
Workflows will be executed by the **SciWIn Compute Servers**, and results, including **full provenance information**, will be passed back to SciWIn Hub which will inform the Scientist. The SciWIn Compute Servers will be able to execute Workflows using state-of-the-art workflow engines such as CWLTool, SnakeMake, Nextflow or Galaxy. However, researches are encouraged to send Workflows in CWL[^7] format.
SciWIn Hub will also communicate with the **FAIRagro Middleware** (Measure 4.2)[^6] which handles bidirectional communication with various data repositories.

Research Objects can contain various different components like data, code, workflows, metadata and provenance each which is optional. ROs can also point to large data (multiple TB) in remote data inventories. By using git ROs and their components will be versioned out of the box.


## Re-usable data handling
Scientists will record ad-hoc workflows for data pre-processing, data transformation or data analysis using the SciWIn Client. By using git, an iterative and **collaborative workflow development**, including version control of data and code, is possible, furhter **improving the overall user experience**. Research objects will be FAIR DOs, making the creation of shareable research objects with provenance information and metadata easy,


## Integration & exploration
As SciWIn Hub contains a collection of ROs, the possibility to explore of research objects (RO) on SciWIn Hub will enable scientists to download parts (code, data, metadata), recombine artifacts in new research objects and upload to SciWIn Hub to integrate new ROs into the RO collection. ROs derived from already existing parts will have their parts point to the original parts to ensure traceability of the creation process. This process could also be called as a mix and match feature.


## Workflow execution
Workflows can be(semi-)automatically transformed into a formal specification like CWL. SciWIn will be compatible with workflow publishing platforms like workflowhub.eu, making collaboration and creation of workflows even easier. Furthermore all major execution engines such as CWLTool, SnakeMake, Nextflow or Galaxy will likely to be supported. 

## FAIR Publication
Workflows will be annotated with metadata (linked data, schema.org) and a unique persistent identifier to make them findable. ROs will also be published by using an existing PID system (DOI, ARK). THe publication of the FAIR DO in an appropriate repository will be brokered by FAIRagro Middleware.

## Roadmap
![Roadmap](./assets/roadmap.svg)


The SciWIn Roadmap as presented in the FAIRagro Proposal starts with the concept phase in early 2024. A proof-of-concept stage will hopefully be reached in late 2026 according to the planned timeframe.

## Download
The presented poster and the slides of the lightning talk can be downloaded by clicking the buttons below (CC-BY 4.0).

**TODO**: nicer & working buttons^^

<kbd>
<br/>
Dowload Poster
<br/><br/>
</kbd>
<kbd>
<br/>
Dowload Slides
<br/><br/>
</kbd>


***

[^1]: **F**indable **A**ccessible **I**nteroperable **R**eusable
[^2]: **C**ommon **W**orkflow **L**anguage
[^3]: **P**ersistant **ID**entifier
[^4]: **D**igital **O**bject **I**dentifier
[^5]: FAIR **D**igital **O**bject
[^6]: Information about Measure 4.2 can be found in the [FAIRagro Proposal](https://doi.org/10.5281/zenodo.8366884)
[^7]: **C**ommon **W**orkflow **L**anguage