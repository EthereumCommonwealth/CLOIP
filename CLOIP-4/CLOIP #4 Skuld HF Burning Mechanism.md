---
cloip: 4
title: Callisto Network Skuld HF Dynamic Monetary Policy
author: Dr ZS (@Dr-ZS)
status: Last Call
category: Core
created: 2023-08-31
---

## Abstract
The Callisto Network's Skuld Hard Fork introduces burning mechanisms, variable block sizes, increased minimum gas fees, and reduced block times to optimize security, scalability, and economic incentives, mirroring some of Ethereum's EIP-1559 features. This document proposes the following blocks at which to implement these changes in the Callisto networks:

13_200_001 on Callisto PoW-mainnet (September 22nd, 2023)

## Motivation
With the blockchain ecosystem's rapid expansion, Layer 1 platforms are encountering significant scalability issues. It's paramount to address these without compromising security and decentralization for wider adoption and longevity. The Callisto Network's Skuld Hard Fork is driven by the necessity to boost platform efficiency, fortify its economic model, and refine user experience, all while ensuring robust security. Furthermore, this initiative capitalizes on emerging edge computing infrastructures and advancements in network connectivity ushered in by 5G and subsequent generations.

## Specification

### 1. Burning Mechanism & Block Reward:

- Implement a dual-fee structure:
  - **Base Fee**: A fee that will be burned and will adjust according to network activity.
  - **Priority Fee**: A separate fee given to miners.

- Shift from a decreasing block reward model to a fixed reward per block to ensure consistent incentives for network participants and control inflation.

### 2. Variable Block Size:

- Instead of a fixed-size block reward, the network will be able to adjust the block size in response to transaction bursts.
- Block gas limit will dynamically adjust between 8 million to 15 million based on network utilization.

### 3. Minimum Gas Fee:

- Establish a minimum transaction cost of 1000 gas.
- Standard transaction cost on the Callisto Network will be set at 0.02 CLO to deter spam transactions while remaining competitive.

### 4. Block Time Reduction:

- Block time will be reduced by approximately 20%.
- This is achieved through adjustments in the difficulty calculation.

### Infrastructure Integration:

- The network's improvements and scalability will leverage edge computing infrastructures.
- Seamless integration and functionality with the enhanced network connectivity features of 5G and beyond networks are anticipated.

## Rationale

### 1. Burning Mechanism & Block Reward:

The introduction of the burning mechanism, especially one akin to Ethereum's EIP-1559, is pivotal for various reasons:

- **Inflation Control**: Burning a portion of transaction fees aids in reducing the potential inflationary pressures caused by the issuance of new tokens.
  
- **Predictable Fee System**: With an adaptive base fee, users can have a more predictable fee estimation, helping them in understanding transaction costs better.

- **Incentivization**: By keeping a fixed reward system, miners and stakers later on have a predictable revenue stream, encouraging consistent participation and ensuring network security.

### 2. Variable Block Size:

Adjustable block size addresses the crucial concern of scalability:

- **Flexibility**: It provides the network the flexibility to accommodate bursts of transactions, especially vital in the era of DeFi platforms where transaction bursts are commonplace.
  
- **Optimized User Experience**: Variable block sizes ensure faster transaction confirmations during peak times, enhancing user experience.

### 3. Minimum Gas Fee:

Implementing a higher minimum gas fee is rationalized by:

- **Network Protection**: By disincentivizing spam transactions, the network ensures efficient use of its resources and better protection against DoS attacks.
  
- **Sustainability**: It balances the need for affordable transactions with the long-term economic sustainability of the network.

### 4. Block Time Reduction:

Reducing block time is geared towards:

- **Enhanced User Experience**: Faster block times translate to quicker transaction confirmations, positively impacting DApp responsiveness and overall user satisfaction.
  
- **Increased Miner Rewards**: As more blocks are minted each day, miners receive more rewards, ensuring their consistent participation.

### Infrastructure Integration:

Capitalizing on edge computing and improved network connectivity offers:

- **Scalability**: Edge computing decentralizes processing and places it closer to transaction sources, allowing for more scalable solutions.
  
- **Speed & Efficiency**: With 5G and subsequent connectivity generations, faster data transfer rates can be achieved, ensuring swift transaction processing and propagation across nodes.

In summary, the Skuld Hard Fork's rationale is grounded in a forward-thinking approach. By addressing the pressing concerns of scalability, economic sustainability, and enhanced user experience while leveraging cutting-edge infrastructure advancements, Callisto Network aims to solidify its position in the blockchain ecosystem.

## Backwards Compatibility

Ensuring backward compatibility is paramount when introducing significant changes to a network. For the Skuld Hard Fork on the Callisto Network, several areas of concern are addressed:

### 1. **Existing Smart Contracts**:
- **Action**: It's essential to confirm that all the proposed changes in the Skuld Hard Fork do not disrupt the operation of existing smart contracts on the Callisto Network.
- **Mitigation**: For contracts that may potentially be affected, it's crucial to provide developers with adequate documentation and tools to help them make necessary adjustments.

### 2. **Wallet and dApp Interactions**:
- **Action**: Considering the close compatibility with Ethereum wallets, any alterations to transaction structures, fee mechanisms, or other elements should not break integrations.
- **Mitigation**: Rigorous testing on testnet environments, ensuring that popular wallets and dApps still function correctly and can recognize and correctly interpret new or modified data structures.

### 3. **Miner Adjustments**:
- **Action**: With changes to block rewards and transaction fees, miners might need to adjust their setups, especially if there's new data they need to process or if the reward mechanisms change significantly.
- **Mitigation**: Distribute clear documentation and possibly software patches or updates to popular mining software that interacts with Callisto.

### 4. **Node and Network Upgrades**:
- **Action**: Nodes will need to upgrade to accommodate the changes introduced in the Skuld Hard Fork.
- **Mitigation**: Ensure that node upgrade processes are as seamless as possible. Provide thorough documentation and support channels for node operators to clarify any doubts and troubleshoot potential issues.

## Simulation Experiments

Simulation experiments play an essential role in assessing the potential outcomes and possible implications of changes proposed in a hard fork. For the Skuld Hard Fork on the Callisto Network, the following experiments were conducted:

### 1. **Transaction Throughput**:
- **Objective**: Measure network's ability under increased transactions.
- **Method**: Simulate high-volume periods on testnet.
- **Results**: Improved transaction processing times.

### 2. **Burn Mechanism Efficiency**:
- **Objective**: Assess burning mechanism's impact on network economics.
- **Method**: Simulate various network utilization scenarios.
- **Results**: Efficient burning, deflationary effect observed.

### 3. **Network Security**:
- **Objective**: Evaluate network security with changes in miner incentives.
- **Method**: Conduct penetration testing on testnet.
- **Results**: No new vulnerabilities introduced.

### 4. **dApp Interaction and Smart Contract Execution**:
- **Objective**: Ensure dApps and smart contracts function with proposed changes.
- **Method**: Execute smart contracts and dApp interactions on testnet.
- **Results**: All dApps and contracts operated as expected.

## Conclusions
The Monetary Policy Hard Fork (codename Skuld) is one of the major components of Callisto Network's strategic plan. Besides limiting inflation in the first step to stopping it in the long run, it provides a higher incentive for miners and maximizes the APR of Cold Stakers and offers an improved user experience to dApp users by further decreasing the latency. It is, therefore, the foundation for upcoming upgrades such as ZPoW or the DAG size reduction.Although the strategic plan initially foresaw a Hard Fork for the last quarter of 2022, in light of the results of the tests, it was decided to extend the testing period by a few weeks to fine-tune every parameter. Several test models are being tested on Callisto Enterprises' private testnets... Skuld is approaching, be prepared! As the Hard Fork is coming, please be prepared to mine and perform transactions over the Callisto Network testnet. Rewards will be distributed to users who will point their GPUs for mining or will interact with the testnet dApps allowing to test in the optimal conditions the proposed optimizations . The exact days will be announced after the testing in our private testnets is finished. 

## Security Considerations

Ensuring the security of the Callisto Network during the Skuld Hard Fork is crucial. Here are the main security considerations for the proposed changes:

### 1. **Variable Size Blocks**:
- **Concern**: Increased vulnerability to spam or flood attacks.
- **Mitigation**: Implementation of minimum gas fee and dynamic block size adjustment.

### 2. **Minimum Gas Fee**:
- **Concern**: Exclusion of users due to higher costs.
- **Mitigation**: Modest increase to deter spam, not genuine users.

### 3. **Block Time Reduction**:
- **Concern**: Increased chances of orphaned blocks and security risks.
- **Mitigation**: Thorough testing and improved consensus mechanisms.

## Copyright

This CLOIP is placed under the [CC0-1.0](https://creativecommons.org/publicdomain/zero/1.0/).
