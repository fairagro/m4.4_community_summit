# SciWIn - A Concept for a FAIR Scientific Workflow Infrastructure
<small>

- Antonia Leidel (Leibniz Institute of Plant Genetics and Crop Plant Research, IPK)
- Dr. Jens Krumsieck (Thünen Institute) [![ORCID: 0000-0001-6242-5846](./_include/orcid.png)](https://orcid.org/0000-0001-6242-5846)
- Patrick König (Leibniz Institute of Plant Genetics and Crop Plant Research, IPK) [![ORCID: 0000-0002-8948-6793](./_include/orcid.png)](https://orcid.org/0000-0002-8948-6793)
- Dr. Harald von Waldow (Thünen Institute) [![ORCID: 0000-0003-4800-2833](./_include/orcid.png)](https://orcid.org/0000-0003-4800-2833)

on behalf of the FAIRagro consortium
</small>


## Introduction

FAIR research is becoming increasingly important, but developing and publishing FAIR workflows can be challenging. A Scientific Workflow Infrastructure (SciWIn) will facilitate collaboration and increase reusability by giving researchers access to workflows that can be combined and extended. SciWIn will also support scientists during development with versioning and help them to formally specify their workflows, making them executable on workflow engines. Detailed documentation will be provided through the use of FAIR Digital Objects (FDOs). 
 

## Concept
- Integration of workflows and data from multiple repositories including a SciWIn Workflow Hub
- Users can access different data environments for workflow development via a central server 
- A stable workflow within a data environment can be (semi-)automatically transformed into a formal workflow specification
- The formal workflow specification can be executed by a workflow engine

## Reusable Data Handling
- The user builds a multi-step workflow for data transformation, modification, pre-processing and integration 
- Iterative development process that includes bug fixes and changes
- Data environment keeps track of different versions and pushes environment to central server
- Central server facilitates collaboration by providing access to organized data environments

## Mix and Match
- View multiple data environments
- Download parts (e.g., code, data, metadata) from different data environments
- Recombine them in new data environment
- Uploaded derived parts that are linked to original parts on the server


## Workflow execution and FAIR publication
- Stable workflows can be (semi-) automatically transformed into a formal specification such as CWL
- Formal specification is compatible with workflow publishing platforms and execution engines 
- Stable workflow is annotated with metadata
- Publication in an appropriate repository with PID system

## Workflow Engines
### SnakeMake
- Workflow management system with domain specific language (DSL) based on Python
- Transformation of input files in multiple steps via shell commands, Python code blocks, external scripts in Python, R or Julia or a Jupyter notebook

### Nextflow
- Workflow management system for scalable and portable workflows
- Independent execution of different processes written in scripting language (e.g. Bash, Python,...) on Linux platform 
