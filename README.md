# Callisto Network Improvement Proposals (CLOIPs)

Callisto Network Improvement Proposals (CLOIPs) are technical documents describing the changes proposed to the Callisto Network protocol. Once finalized and approved by the core developers, volunteer client developers, implementers, and other users of Callisto Network, proposals are implemented by the core developer team.

Each proposal will be reviewed and discussed by the core and volunteer developers of Callisto Network and any developers willing to contribute their motivated opinions.

## Contributing

To submit a proposal, you can clone the repository and add your CLOIP. A CLOIP template is available [here](/CLOIP-template.md). Then submit a Pull Request to Callisto Network’s CLOIPs repository.

## CLOIP status terms

- **Idea** - An idea that is pre-draft. This is not tracked within the EIP Repository.
- **Draft** - The first formally tracked stage of an EIP in development. An EIP is merged by an EIP Editor into the EIP repository when properly formatted.
- **Review** - An EIP Author marks an EIP as ready for and requesting Peer Review.
- **Last Call** - This is the final review window for an EIP before moving to FINAL. An EIP editor will assign the Last Call status and set a review end date (`last-call-deadline`), typically 14 days later. If this period results in necessary normative changes, it will revert the EIP to Review.
- **Final** - This EIP represents the final standard. A Final EIP exists in a state of finality and should only be updated to correct errata and add non-normative clarifications.
- **Stagnant** - Any EIP in Draft or Review if inactive for a period of 6 months or greater is moved to Stagnant. An EIP may be resurrected from this state by Authors or EIP Editors by moving it back to Draft.
- **Withdrawn** - The EIP Author(s) have withdrawn the proposed EIP. This state has finality and can no longer be resurrected using this EIP number. If the idea is pursued at later date, it is considered a new proposal.
- **Living** - A special status for EIPs that are designed to be continually updated and not reach a state of finality. This includes, most notably, EIP-1.

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

