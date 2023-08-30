---
cloip: 3
title: Skuld HF
author: Dr ZS (@Dr-ZS)
status: Last Call
category: Core
created: 2023-08-31
---

## Simple Summary  
Enable the Ethereum Foundation Berlin network protocol upgrades on the Callisto network in a hard-fork code-named Skuld HF to enable maximum compatibility across Eth based networks and prepare the transition to Proof of Stake consensus mechanism.

## Abstract  
Introduce a selection of protocol-related modifications that were initially presented in the Ethereum Foundation's (ETH) Berlin hardforks. The suggested updates for the Skuld Hardfork upgrade on the Callisto network are as follows

- Reprices the gas cost of the ModExp (0x00..05) precompile.
- Increases gas cost for SLOAD, *CALL, BALANCE, EXT*, and SELFEDESTRUCT when used for the first time in a transaction.
- Defines a new transaction type that is an envelope for future transaction types.
- Adds a transaction type which contains an access list, a list of addresses and storage keys that the transaction plans to access.

This document proposes the following blocks at which to implement these changes in the Callisto networks:

- 13_200_001 on Callisto PoW-mainnet (September 22nd, 2023)

For more information on the opcodes and their respective EIPs and implementations, please see the **Specification** section of this document.

## Motivation  
To enhance the Ethereum Virtual Machine’s (EVM) capabilities, various opcodes shall be added to the Callisto network, all of which have been in use on the Ethereum Foundation networks since early 2021.

## Specification  
Technical specifications for each EIP can be found at those documents respectively:

- [EIP-2565: ModExp Gas Cost](https://eips.ethereum.org/EIPS/eip-2565)
- [EIP-2929: Gas cost increases for state access opcodes](https://eips.ethereum.org/EIPS/eip-2929)
- [EIP-2718: Typed Transaction Envelope](https://eips.ethereum.org/EIPS/eip-2718)
- [EIP-2930: Optional access lists](https://eips.ethereum.org/EIPS/eip-2930)

## Rationale  
- Interoperability: Establishing and maintaining interoperable behavior between Ethereum clients is essential for developers and end-user adoption, yielding benefits for all participating chains (e.g., ETH and Callisto).
- Immutability: None of the introduced new opcodes in the EVM has the potential to change the behavior of existing contracts; in the case where previously an arbitrary invalid bytecode would have been deployed to the network, none of them would be able to modify the state of the Callisto networks retrospectively. Adding opcodes to the EVM increases its functionality and should be considered a feature upgrade rather than a modification.
