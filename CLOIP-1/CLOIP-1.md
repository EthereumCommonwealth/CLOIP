---
cloip: 1
title: Purpose and Guidelines for CLOIP
author: Dr ZS (@Dr-ZS)
status: Living
type: Meta
created: 2023-07-26
---

## Introduction to CLOIP

CLOIP, short for Callisto (CLO) Network Improvement Proposal, serves as a blueprint that offers detailed information to the Callisto Network community about new feature proposals for Callisto Network, its processes, and environment. Each CLOIP should encapsulate a well-defined technical specification of the feature, coupled with its rationale. The author of the CLOIP takes the responsibility to foster consensus within the community and to document contrary opinions.

## Significance of CLOIP

CLOIPs are envisioned to be the pivotal mechanisms for the proposal of new features, accumulation of community technical input on issues, and documentation of the design decisions within Callisto Network. The CLOIPs, being maintained as text files in a versioned repository, also serve as the historical record of feature proposals.

For the implementers of Callisto Network, CLOIPs provide a convenient method to keep track of the progress of their implementation. It would be beneficial if each implementation maintainer lists the CLOIPs they have implemented. This practice will provide end users with an easy way to stay updated on the status of a particular implementation or library.

## Classification of CLOIPs

CLOIPs can be classified into three categories:

- **Standards Track CLOIP:** Describes any alteration that affects most or all Callisto Network implementations. This could involve changes to the network protocol, block or transaction validity rules, proposed application standards or conventions, or any addition or modification that impacts the interoperability of applications utilizing Callisto Network. Standards Track CLOIPs are further categorized into:
  - **Core:** Encompasses improvements requiring a consensus fork, along with changes that aren't necessarily consensus critical.
  - **Networking:** Includes improvements around networking protocols and strategies.
  - **Interface:** Comprises improvements around client specifications and standards, and certain language-level standards like method names. Discussion regarding this category should primarily occur in the [interfaces repo] before an CLOIP is submitted to the CLOIPs repository.
  - **ERC:** Application-level standards and conventions, including contract standards, name registries, URI schemes, library/package formats, and wallet formats.

- **Meta CLOIP:** Describes a process around Callisto Network or proposes a change to (or an event in) a process. Unlike Informational CLOIPs, they are more than mere recommendations, and users are typically obligated to adhere to them.

- **Informational CLOIP:** Describes a Callisto Network design issue or offers general guidelines or information to the Callisto Network community, without proposing a new feature.

A single CLOIP should ideally contain a single key proposal or new idea. The more focused the CLOIP, the more successful it tends to be. A change to one client doesn't warrant a CLOIP; however, a change that affects multiple clients or defines a standard for multiple apps to use, does require a CLOIP.

### Special Requirements for Core CLOIPs

Any Core CLOIP that mentions or proposes modifications to the EVM (Callisto Network Virtual Machine) should specify the instructions by their mnemonics and define the opcodes at least once. A preferred format is as follows:
REVERT (0xfe)


## CLOIP Workflow
## CLOIP Workflow

The CLOIP process begins with an idea for improving the Callisto Network. These improvement ideas can range from core protocol changes, to the applications, frameworks, and protocols built on top of the Callisto Network, and even organizational changes or improvements.

Here's a detailed explanation of each status a CLOIP may have:

- **Idea**: This represents an idea that is pre-draft. This stage is not tracked within the CLOIP Repository.

- **Draft**: The first formally tracked stage of a CLOIP in development. A CLOIP is merged by a CLOIP Editor into the CLOIP repository when properly formatted.

- **Review**: A CLOIP Author marks a CLOIP as ready for and requesting Peer Review.

- **Last Call**: This is the final review window for a CLOIP before moving to Final. A CLOIP editor will assign Last Call status and set a review end date (last-call-deadline), typically 14 days later. If this period results in necessary normative changes it will revert the CLOIP to Review.

- **Final**: This CLOIP represents the final standard. A Final CLOIP exists in a state of finality and should only be updated to correct errata and add non-normative clarifications. A PR moving a CLOIP from Last Call to Final SHOULD contain no changes other than the status update. Any content or editorial proposed change SHOULD be separate from this status-updating PR and committed prior to it.

- **Stagnant**: Any CLOIP in Draft, Review, or Last Call that has been inactive for a period of 6 months or greater is moved to Stagnant. A CLOIP may be resurrected from this state by Authors or CLOIP Editors through moving it back to Draft or its earlier status. If not resurrected, a proposal may stay forever in this status. CLOIP Authors are notified of any algorithmic change to the status of their CLOIP.

- **Withdrawn**: The CLOIP Author(s) have withdrawn the proposed CLOIP. This state has finality and can no longer be resurrected using this CLOIP number. If the idea is pursued at a later date, it is considered a new proposal.

- **Living**: A special status for CLOIPs that are designed to be continually updated and not reach a state of finality.

Below is a diagram that illustrates the CLOIP process:

![CLOIP Status Diagram] [link]

Please remember that making a CLOIP does not guarantee that it will be implemented. That decision is left up to the individual project maintainers.


### Shepherding a CLOIP

The process involves you, the CLOIP author, and the CLOIP editors. 

Before formalizing a CLOIP, you should validate your idea with the Callisto Network community to avoid redundancy. We recommend initiating a discussion thread on the official Telegram channel [Link].

Following validation, your responsibility will be to present your CLOIP to reviewers, invite editors, developers, and the community to provide feedback on the dedicated channels.

### Core CLOIPs

For Core CLOIPs to be considered Final, you will need to either provide an implementation for clients or convince clients to implement your CLOIP.


## CLOIP Formats and Templates

CLOIPs should be authored in markdown format. A template is available (https://github.com/EthereumCommonwealth/CLOIP/blob/main/CLOIP-template.md).

## CLOIP Editors and Their Responsibilities

The current CLOIP editors include:

- DR_ZS(@Dr-ZS)
- Tonton (@spatialiste)
- Dexaran (@dexaran)

CLOIP editors perform an initial review of the CLOIP for completeness, clarity, technical soundness, title accuracy, language, and markup. If the CLOIP is not ready, it will be returned to the author for revision. Once the CLOIP is deemed ready, the editor will assign an CLOIP number and merge the corresponding pull request.

## Style Guide

CLOIP authors are encouraged to follow specific guidelines for titles, descriptions, and CLOIP numbers, and to adhere to the terminologies as described in RFC 2119 and RFC 8174.

## History

This document draws heavily from Bitcoin's BIP-0001, Python's PEP-0001 and Ethereum's EIP-001. In many instances, the text was directly copied and modified.

## Copyright

Copyright and related rights waived via [CC0](../LICENSE.md).

