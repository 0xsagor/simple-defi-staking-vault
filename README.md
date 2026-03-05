# Simple DeFi Staking Vault

A high-performance, professional implementation of a staking vault. This repository provides a secure way for users to lock their digital assets and accrue rewards based on time and pool weight.

## Features
* **Proportional Rewards:** Rewards are calculated based on the user's percentage of the total staked supply.
* **Security First:** Uses `ReentrancyGuard` to prevent common smart contract vulnerabilities.
* **Emergency Controls:** Includes owner-only functions for managing reward distributions.

## Getting Started
1. Install dependencies: `npm install`.
2. Deploy the `StakingVault.sol` by passing the address of the ERC-20 token to be staked.
3. The owner must call `notifyRewardAmount` to fund the reward pool.
4. Users can then `stake`, `withdraw`, and `getReward`.

## License
MIT
