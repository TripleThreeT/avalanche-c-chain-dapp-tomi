# Avalanche Fuji C-Chain ERC-20 Internship Task

## Overview
Deployed a simple ERC-20 token (`TomiInternToken` / TINT) on the **Avalanche Fuji testnet** using **Core Wallet** and **Remix IDE**.

## Wallet Setup
- Core Wallet (extension/app)  
- Testnet mode enabled (see screenshot)  
- Received 2 test AVAX via Core faucet  
- Connected to Remix via Injected Provider - Core

## Contract Details
- **Name**: TomiInternToken  
- **Symbol**: TINT  
- **Decimals**: 18  
- **Contract Address**: `0xEA09a0e79aAC362054A832233b5F15B38080Eb70`  
- **Features**: Mintable (owner only), Ownable, premint 1,000,000 tokens to deployer  
- **Explorer**: https://testnet.snowtrace.io/address/0xEA09a0e79aAC362054A832233b5F15B38080Eb70

## Tools & Process
- **Development environment**: Core Wallet + Remix IDE  
- **Compiler**: Solidity 0.8.31+ with EVM version cancun  
- **Deployment**: Injected Provider - Core → Deploy button → approved in Core  
- **Interactions**: Read (name, symbol, balanceOf) and write (mint, transfer) functions called directly in Remix  
- **Gas fees**: ~0.001–0.004 AVAX per tx (very low on testnet)

## Proof of Successful Transactions
See `/screenshots/` folder:
- Wallet balance & testnet confirmation
- Contract page on Snowtrace
- Full transaction history (deployment, mint, transfer)

## How to Verify
1. Visit the contract on Snowtrace: [link above]
2. Check the 3 transactions:
   - Contract Creation (deployment)
   - Mint
   - Transfer

All txs are successful on Fuji testnet.

## What I Learned
- Gas on Fuji testnet is extremely low (~0.001–0.004 AVAX per tx) compared to mainnet expectations
- Finality feels near-instant (txs confirm in seconds)
- Injected providers (Core Wallet → Remix) make deployment and interaction seamless without manual RPC setup
- Seedless wallets in Core are secure but limit private key export — Remix direct interaction works perfectly

Built for Avalanche internship task – February 2026
