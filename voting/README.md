# Voting Contract

This contract facilitates a decentralized voting mechanism, primarily for validators to collectively decide on critical actions, such as unlocking token transfers. It is designed to ensure that decisions are made with significant consensus from the participating stakeholders.

## How it Works

1.  **Voting Mechanism**: Validators can cast their vote by calling the `vote` function, specifying the amount of stake they wish to commit to their vote. This stake represents their conviction in the decision.
2.  **Consensus Threshold**: The voting process concludes when more than two-thirds (2/3) of the total staked amount at any given moment has voted in favor of a proposal. This supermajority threshold ensures robust agreement before any action is taken.
3.  **Immutability After Vote**: Once the voting threshold is met and the voting is finalized, the contract enters an immutable state. This means no further modifications or votes can be cast, ensuring the integrity and finality of the decision.

## Use Cases

*   **Token Transfer Unlocking**: The primary use case is to collectively decide on unlocking token transfers, providing a secure and decentralized way to manage critical protocol parameters.
*   **Decentralized Governance**: This contract can be adapted for various decentralized governance scenarios where a supermajority consensus is required for significant protocol changes or actions.

This contract ensures a secure, transparent, and decentralized decision-making process, leveraging the power of staked assets to achieve consensus.
