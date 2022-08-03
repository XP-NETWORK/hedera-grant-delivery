
# DONE

## Milestone 1 — Smart Contract Development & Deployment

Length - 1 week - DONE

0. Research about Hedera standards and other factors & [protocols](https://docs.hedera.com/guides/core-concepts/smart-contracts/supported-erc-token-standards) that distinguish it from other chains<br/>
We will develop smart contracts that will:

1. [Add](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/f474704150da557f931e011026d0c033b391bd7a/dist/Minter.d.ts#L221-L223) / [Remove](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/f474704150da557f931e011026d0c033b391bd7a/dist/Minter.d.ts#L227-L229) a validator
2. [Freeze](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/f474704150da557f931e011026d0c033b391bd7a/dist/Minter.d.ts#L164)/[Unfreeze](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/dist/dist/Minter.d.ts#L239-L244) Native NFTs
3. [Mint](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/dist/dist/Minter.d.ts#L186-L188)/[Burn](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/dist/dist/Minter.d.ts#L257-L259) wrapped NFTs
4. [Withdraw](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/dist/dist/Minter.d.ts#L198-L200) the TX fees on the target chain in native tokens
5. [Trust](https://github.com/XP-NETWORK/web3-contracts/blob/erc1155/contracts/Minter.sol#L86-L119) the multisig of the bridge oracle validators
6. [Whitelist](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/dist/dist/Minter.d.ts#L333-L335) NFT smart contracts
7. [Pause](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/dist/dist/Minter.d.ts#L224-L226)/[Unpause](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/dist/dist/Minter.d.ts#L245-L247) for maintenance or if compromised
8. [Reimburse](https://github.com/XP-NETWORK/XP.network-HECO-Migration/blob/dist/dist/Minter.d.ts#L201-L203) the bridge validators their expenses

# TODO:

## Milestone 2 — Integrating into the Live Bridge
Length - 3 weeks

1. Developing validation logic relevant for the Hedera part of the bridge - DONE
2. Adding Hedera to the Bridge NFT-Indexer - Partially DONE
3. Integrating TX fee estimation - Partially DONE
4. Integrating with a Hedera rpc node
5. Integrating Hedera in the bridge UI
6. Deploying smart contracts to the testnet - DONE:
   1. Bridge: https://hashscan.io/#/testnet/contract/0.0.47756643
   2. erc1155Minter: https://hashscan.io/#/testnet/contract/0.0.47756597
   3. Default-ERC-1155: https://hashscan.io/#/testnet/contract/0.0.47756624
   4. ERC-721-Minter: https://hashscan.io/#/testnet/contract/0.0.47756586
   5. Default-ERC-721: https://hashscan.io/#/testnet/contract/0.0.47756610
7. Adding Hedera to the bridge [JS library](https://github.com/XP-NETWORK/xpjs/search?q=hedera) - DONE
8.  Adding access to Hedera from the REST API
9. Adding Hedera to the bridge widget

## Milestone 3 — Testing, Fixing Bugs & Documenting
Length - 1 week 

1. We will provide both inline documentation of the code and a basic tutorial that can interact with the deployed smart contracts and backend service.
2. The code will have proper unit-test coverage 85% to ensure functionality and robustness. In the guide, we will describe how to run these tests preparing for auditing
3. Deploying and testing the contracts in the testnet environment

## Milestone 4 — Mainnet Integration & Deployment
Length - 1 week 

1. Deploying the contracts in the Mainnet environment
2. Integrating the mainnet Wallet
3. Integrating the mainnet NFT-Indexer
4. Integrating the mainnet validators
5. Plugging Hedera in the heartbeat
6. Testing the Integrated Hedera in the mainnet