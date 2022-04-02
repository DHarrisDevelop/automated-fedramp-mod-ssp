# Design Decisions
- We will be working from the [FedRAMP moderate baseline SSP template](https://www.fedramp.gov/assets/resources/templates/FedRAMP-SSP-Moderate-Baseline-Template.docx) provided on [FedRAMP.gov](https://fedramp.gov)
    - The SSP can be broken into sections/objects. In Section 13 minimum security controls each control family has several parts:
        - **Control Requirement**: This is the text from the applicable NIST SP 800-53 control enhnaced with FedRAMP specified requirements
        - **Control Summary Information**: This is a table summarizing the control implentation at the Cloud Service Provider
        - **Solution Summary**: This is a table describing the implementation of the Control Requirements
- We will be using [ASCiiDoctor](https://docs.asciidoctor.org/) to combine files/produce SSP output

## Repo Structure
- **ORGANIZATION** - holds organization specific information, in the SSP section 13 this includes the **Control Summary Information** and the **Solution Summary**
- **STANDARDS** - holds the NIST, FedRAMP, and other applicable requirements for the system
- **SSP** - this holds the information necessary to dynamically generate the SSP. This directory combines information from **STANDARDS**, **ORGANIZATION**, and other places