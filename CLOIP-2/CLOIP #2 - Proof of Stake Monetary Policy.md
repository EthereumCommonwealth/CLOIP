---
cloip: 2
title: Callisto Network Proof of Stake Monetary Policy
author: Dr ZS (@Dr-ZS)
status: Last Call
category: Core
created: 2023-07-17
---

## Abstract

Callisto Network is transitioning to a Proof of Stake consensus to enhance energy efficiency and security. This proposal introduces changes to the Monetary Policy (MP) aimed at incentivizing network decentralization and enhancing its value.

## Motivation

The transition of Callisto Network to a Proof of Stake (PoS) consensus mechanism necessitates a Monetary Policy (MP) ensuring fair distribution of rewards among validators, increased network security, and enhanced decentralization through appropriate economic incentives.

## Specification

The proposal introduces a new structure of network operation with time divided into slots. Validators are randomly selected among the available ones, given the number of coins at stake. Rewards consist of a fixed base reward and a reward per proposer for different operations. Four types of rewards are proposed: (i) Block proposed, (ii) Correct attestation, (iii) Timely attestation, (iv) Whistleblower.

A hard cap of 200,000 CLO coins is suggested for the stake of each validator, promoting decentralization and network security. The maximum emission per year is defined as: Max Annual Emission=1115000*sqrt(N), where N is the number of active validators. 

To preserve the Callisto Network treasury, 10% of validators' rewards are allocated directly to the treasury.

## Rationale

The proposal is designed to allow the rewards to be proportional to the validators' stakes rather than fixed per block. The new structure promotes increased decentralization and network security. The reward distribution is balanced to incentivize participation and disincentivize attacks, leading to a stable and secure network.

## Backwards Compatibility

This EIP does not introduce any known backward compatibility issues.

## Simulation Experiments

In our simulations, we evaluated the potential benefits of the proposed Monetary Policy compared to the existing policy.

### A. Maximum Issuance and APR

We examined the maximum issuance for different numbers of validators. The APR, which depends on the number of coins at stake and the rewards distributed for different numbers of validators, is as follows: 


![Max Issuance](/CLOIP-2/Images/max_issuance.svg)

![APR](/CLOIP-2/Images/APR.svg)

### B. Pow vs. PoS for Different Staking Requirements

We evaluated the potential implementation of a Proof-of-Stake (PoS) system within the Callisto Network, comparing it against the current Proof-of-Work (PoW) monetary policy. 

A critical parameter is the maximum circulating supply. We compared the current PoW emission with the PoS under evaluation by Callisto Network for different numbers of validators. 

![POS vs POW](/CLOIP-2/Images/POSvsPOW.svg)

## Conclusions

Based on our simulations, migrating from a Proof-of-Work to a Proof-of-Stake system for Callisto Network could significantly change coin emission rates. This could amplify the efficiency of the upcoming burning mechanism, driving a greater deflationary trend, potentially increasing the value of each coin, and incentivizing validators within the Callisto Network by increasing their potential rewards.

## Security Considerations

The security of the PoS mechanism is maintained through in-built penalties or "slashing" for validators attempting to act maliciously. Also, the low stakes requirement of 200,000 CLO to run a validator strengthens network security by making it more costly for malicious parties to launch an attack, while also promoting network decentralization.

## Copyright

This CLOIP is placed under the [CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/).
