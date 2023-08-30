# Callisto Network Improvement Proposals (CLOIPs)

Callisto Network Improvement Proposals (CLOIPs) are technical documents describing the changes proposed to the Callisto Network protocol. Once finalized and approved by the core developers, volunteer client developers, implementers, and other users of Callisto Network, proposals are implemented by the core developer team.

Each proposal will be reviewed and discussed by the core and volunteer developers of Callisto Network and any developers willing to contribute their motivated opinions.

## Contributing

To submit a proposal, you can clone the repository and add your CLOIP. A CLOIP template is available [here](/CLOIP-template.md). Then submit a Pull Request to Callisto Network’s CLOIPs repository.

## CLOIP status terms

- **Idea** - An idea that is pre-draft. This is not tracked within the CLOIP Repository.
- **Draft** - The first formally tracked stage of a CLOIP in development. A CLOIP is merged by an CLOIP Editor into the CLOIP repository when properly formatted.
- **Review** - A CLOIP Author marks a CLOIP as ready for and requesting Peer Review.
- **Last Call** - This is the final review window for an CLOIP before moving to FINAL. A CLOIP editor will assign the Last Call status and set a review end date (`last-call-deadline`), typically 14 days later. If this period results in necessary normative changes, it will revert the CLOIP to Review.
- **Final** - This CLOIP represents the final standard. A Final CLOIP exists in a state of finality and should only be updated to correct errata and add non-normative clarifications.
- **Stagnant** - Any CLOIP in Draft or Review if inactive for a period of 6 months or greater is moved to Stagnant. An CLOIP may be resurrected from this state by Authors or CLOIP Editors by moving it back to Draft.
- **Withdrawn** - The CLOIP Author(s) have withdrawn the proposed CLOIP. This state has finality and can no longer be resurrected using this CLOIP number. If the idea is pursued at later date, it is considered a new proposal.
- **Living** - A special status for CLOIPs that are designed to be continually updated and not reach a state of finality. This includes, most notably, CLOIP-1.

## CLOIP Types

CLOIPs are separated into a number of types, and each has its own list of CLOIPs.

### Standard Track
Describes any change that affects most or all Callisto Network implementations, such as a change to the network protocol, a change in block or transaction validity rules, proposed application standards/conventions, or any change or addition that affects the interoperability of applications using Callisto Network.

Standard CLOIPs can be broken down into the following categories:

- **Core**: Improvements requiring a consensus fork, as well as changes that are not necessarily consensus critical but may be relevant to “core dev” discussions.
- **Networking**: Improvements to networking protocol specifications.
- **Interface**: Includes improvements around client API/RPC specifications and standards, and also certain language-level standards like method names and contract ABIs. The label “interface” aligns with the interfaces repo, and discussion should primarily occur in that repository before a CLOIP is submitted to the CLOIPs repository.
- **ERC**: Application-level standards and conventions, including contract standards such as token standards, name registries, URI schemes, library/package formats, and wallet formats.
- **Meta**: Describes a process surrounding Callisto Network or proposes a change to (or an event in) a process. Process CLOIPs are like Standards Track CLOIPs but apply to areas other than the Callisto Network protocol itself. They may propose an implementation, but not to Callisto Network’s codebase; they often require community consensus; unlike Informational CLOIPs, they are more than recommendations, and users are typically not free to ignore them. Examples include procedures, guidelines, changes to the decision-making process, and changes to the tools or environment used in Callisto Network development. Any meta-CLOIP is also considered a Process CLOIP.

### Informational

Describes a Callisto Network design issue or provides general guidelines or information to the Callisto Network community but does not propose a new feature. Informational CLOIPs do not necessarily represent Callisto Network community consensus or a recommendation, so users and implementers are free to ignore Informational CLOIPs or follow their advice.

## Callisto Network CLOIP Contribution Rewards

To encourage innovation and constructive dialogue within the community, Callisto Network is introducing a reward scheme for the most valuable contributions to the Callisto Network Improvements Proposals (CLOIP). The Callisto Network Treasury will grant the rewards.

The rewards structure is as follows:

### Outstanding Comprehensive Contribution - $300 

This reward is granted to the contributor who provides an exceptional and comprehensive contribution to an existing CLOIP.

To qualify, a contribution should include:
* A detailed analysis of the proposal
* Comprehensive feedback
* Alternative solutions (if applicable)

### Insightful Critical Analysis - $150 

This reward is granted to the contributor who provides an insightful and valuable critical analysis of an existing CLOIP.

To qualify, a contribution should include:
* A description of the potential challenges
* Areas for improvement
* Impact analysis

### Extra Reward - $50 

This reward is awarded for the contribution that, in addition to providing a detailed analysis or proposal, outlines a practical implementation strategy for the proposed change.

## Participation Rules:

* Contributions are accepted from the "Draft" up to the "Last Call" stages.
* All contributions and proposals must be original. Any plagiarism will result in disqualification.
* Only the most insightful, detailed, and outstanding contributions will be considered for rewards.
* The decision for reward allocation is solely at the discretion of the CLOIP editors.
* Rewards are paid in CLO, equivalent to the stated USD amounts.
* Authors of rewarded contributions will be announced on the respective CLOIP when the proposal reaches its 'Final' stage.

## Community discussion

This repo is created to track the track the Callisto Improvement Proposals (CLOIP). Community members  can provide their feature requests, feedback, and issue reports commenting on the "issues" section of the respective CLOIP. 

### Submitting a Comment

To submit a comment, proposal, feature request, bug report, or any other feedback, please follow the steps below:

1. Register a Github account.
2. Navigate to the [EthereumCommonwealth/CLOIP/issues](https://github.com/EthereumCommonwealth/CLOIP/issues) page.
3. Find and select the relevant CLOIP thread you wish to comment on.
4. Describe your feedback.
6. Submit new **Comment**.

The received feedback will be discussed in the respective issue thread.
