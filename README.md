<br />
<img src="https://.png" width="500"/>
<br />

SkySwap is a peer-to-peer trading network for Ethereum tokens, initially built on the [Swap Protocol](https://swap.tech/whitepaper/). The SkySwap product family includes [Explorer], [DexIndex](https://dexindex.io/), [SkySwap Instant], and [SkySwap Trader]. This repository contains smart contracts and JavaScript packages for use by developers and traders on the AirSwap network.

[![CircleCI](https://circleci.com/gh/airswap/airswap-protocols.svg?style=svg&circle-token=73bd6668f836ce4306dbf6ca32109ddbb5b7e1fe)](https://circleci.com/gh/airswap/airswap-protocols)

## Smart Contracts

Packages are versioned based on deploys. Major versions e.g. `1.x.x` are mainnet deploys, while minor versions e.g. `x.1.x` are rinkeby deploys. Packages that are not deployed increment patch versions e.g. `x.x.1`. Each package that includes a deployment includes the ABI files for that deployed contract in `builds/contracts` within the package.

REWRITE ME TO CHANGE ME FROM AIRSWAP TO SKYSWAP BELOW THIS POINT:
--------======================================------------------------

| Package                                   | Version                                                                                                     | Description                         |
| :---------------------------------------- | :---------------------------------------------------------------------------------------------------------- | :---------------------------------- |
| [`@airswap/swap`](/source/swap)           | [![npm](https://img.shields.io/npm/v/@airswap/swap)](https://www.npmjs.com/package/@airswap/swap)           | Atomic Swap Between Tokens          |
| [`@airswap/indexer`](/source/indexer)     | [![npm](https://img.shields.io/npm/v/@airswap/indexer)](https://www.npmjs.com/package/@airswap/indexer)     | Counterparty Discovery with Staking |
| [`@airswap/delegate`](/source/delegate)   | [![npm](https://img.shields.io/npm/v/@airswap/delegate)](https://www.npmjs.com/package/@airswap/delegate)   | Onchain Trading Delegate            |
| [`@airswap/validator`](/source/validator) | [![npm](https://img.shields.io/npm/v/@airswap/validator)](https://www.npmjs.com/package/@airswap/validator) | Validation and Pre-Swap Checks      |
| [`@airswap/wrapper`](/source/wrapper)     | [![npm](https://img.shields.io/npm/v/@airswap/wrapper)](https://www.npmjs.com/package/@airswap/wrapper)     | Use ether for WETH trades           |
| [`@airswap/types`](/source/types)         | [![npm](https://img.shields.io/npm/v/@airswap/types)](https://www.npmjs.com/package/@airswap/types)         | Types and Hashes                    |
| [`@airswap/transfers`](/source/transfers) | [![npm](https://img.shields.io/npm/v/@airswap/transfers)](https://www.npmjs.com/package/@airswap/transfers) | Token Transfer Handlers             |
| [`@airswap/tokens`](/source/tokens)       | [![npm](https://img.shields.io/npm/v/@airswap/tokens)](https://www.npmjs.com/package/@airswap/tokens)       | Ethereum Tokens                     |

## JavaScript Libraries

| Package                                  | Version                                                                                                     | Description           |
| :--------------------------------------- | :---------------------------------------------------------------------------------------------------------- | :-------------------- |
| [`@airswap/protocols`](/tools/protocols) | [![npm](https://img.shields.io/npm/v/@airswap/protocols)](https://www.npmjs.com/package/@airswap/protocols) | Protocol Clients      |
| [`@airswap/utils`](/tools/utils)         | [![npm](https://img.shields.io/npm/v/@airswap/utils)](https://www.npmjs.com/package/@airswap/utils)         | Orders and Signatures |
| [`@airswap/metadata`](/tools/metadata)   | [![npm](https://img.shields.io/npm/v/@airswap/metadata)](https://www.npmjs.com/package/@airswap/metadata)   | Metadata Management   |
| [`@airswap/constants`](/tools/constants) | [![npm](https://img.shields.io/npm/v/@airswap/constants)](https://www.npmjs.com/package/@airswap/constants) | Helpful Constants     |

## Commands

| Command        | Description                                                                   |
| :------------- | :---------------------------------------------------------------------------- |
| `yarn compile` | Compile all contracts to `build` folders.                                     |
| `yarn clean`   | Delete all contract `build` folders.                                          |
| `yarn ganache` | Run a local `ganache` network on local host 8545.                             |
| `yarn test`    | Run all contract tests in `test` folders. Run `yarn ganache` elsewhere first. |
| `yarn hint`    | Run a syntax linter for all Solidity code.                                    |
| `yarn lint`    | Run a syntax linter for all JavaScript code.                                  |
| `yarn deps`    | Run a dependency consistency check.                                           |

## Deployments

To deploy, please follow [this guide](./tools/deployer)
