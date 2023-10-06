---
cloip: 5
title: Management of media resources on Callisto Network
author: Dexaran (@Dexaran) <dexaran@callisto.network>
status: Final
category: Meta
created: 2023/10/06
---

## Abstract

This CLOIP describes a core tool on Callisto Network that is intended to store a list of "official" media resources on chain. In case of any disputes the list of media resources stored in the on chain registry must be considered valid.

This CLOIP is an implementation of [ECIP-93](https://github.com/ethereumproject/ECIPs/issues/93) proposed in 2019 to Ethereum Classic community. Description can be found at [EthereumCommonwealth Roadmap announcement 68](https://github.com/EthereumCommonwealth/Roadmap/issues/68).

## Motivation
Decentralization is one of the basic concepts of the crypto industry. Nevertheless, the following aspects of any projects are fully centralized and can be easily censored:

- Logo
- Branding/Project name
- Official twitter account
- Official reddit
- Official Slack/Discord live chat
- Github repositories and source codes
- Official emails

Most media resources have owners who can determine the fate of the project by forming public opinion. Of course, the official logo and the name of the project are not so important. However, many decisions in the community are taken not by the community itself, but by a group of people who control official media resources, i.e. which can make the "official announcement".

When it comes to making such critical decisions as performing a hardfork, it is necessary to notify exchanges and mining pools. In the end, whether hardfork will occur or not, depends on the exchange and pools that will support it or not. In many respects success depends on WHO will announce the forthcoming hardfork for the community and WHO will notify the exchanges (WHO = what media and whether they are "official" or not).

On the other hand, in a decentralized community there should not be unequivocally official resources, as any member of the community is as much official as the others.

The key issue here is who to consider to be "official", i.e. who has a permission to speak on behalf of the whole decentralized community.

The community can not make a decision on what media resources of this project are considered official and which are not. The community also can not express disagreement and change one of the resources if the interests of the owner of this resource are at conflict with the interests of the community.

## Specification

#### Deployment

Contract on Callisto mainnet: [0xf6f29E5ba51171C4eF4997bD0208C7E9bc5D5edA](https://explorer.callisto.network/address/0xf6f29E5ba51171C4eF4997bD0208C7E9bc5D5edA/transactions)

UI: https://checker.callisto.network/

Backup UI: https://ethereumcommonwealth.github.io/callisto-officiality-checker/

In order to identify which resource is considered "valid" one must query the contract or paste a link in the UI.

#### Implementation

This proposal introduces a [Media Resources Registry](https://github.com/Dexaran/media-resources-registry/blob/master/MediaRegistry.sol) smart-contract. This contract is intended to preserve a list of official resources that are approved by the community on-chain without 3d party interference.

This contract has a couple of methods [add_entry](https://github.com/Dexaran/media-resources-registry/blob/master/MediaRegistry.sol#L25) and [remove_entry](https://github.com/Dexaran/media-resources-registry/blob/master/MediaRegistry.sol#L34) which serve to add/remove official resources.

It should be considered that only those resources that are currently represented in the described contract are official and are approved by the community.

#### Anti-Scam protection

This proposal can also improve the protection against scam websites and non-official links that can hurt users. It is possible to [query the contract](https://github.com/Dexaran/media-resources-registry/blob/master/MediaRegistry.sol#L48) to ensure whether a given link is registered as an official resource or not.

It is also possible to create a user-friendly web UI that will represent this information. This can help to avoid confusion and uncertainty about what resources provide officially reliable information because fraudsters rely on this uncertainty to deceive users.

#### Updating process of the Media Resources Registry

As the ecosystem and technologies are quickly evolving it may become necessary to upgrade the Media Resources Registry at some point. The contract can not be updated so the only way of updating the registry is to deploy a new one. In order for a new version to become "official" it must be validated by the previous one. The older version of the Media Resources Registry contract must be emptied upon the updating process i.e. it's records must be erased and the only record in the older registry must be a link to the new registry.

The process of Media Resources Registry upgrade:

1. Deployment of a new registry
2. Filling new registry with records of "official" resources
3. Validation of the new registry by the old registry (a record of new registry address must be added to the old registry as "official resource")
4. Emptying of the old registry (all records except the record of a new registry must be erased)


## Copyright

This CLOIP is placed under the [CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/).
