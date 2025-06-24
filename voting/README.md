# Voting Contract

This contract facilitates a decentralized voting mechanism primarily for validators to decide on critical actions, such as unlocking token transfers. It ensures that decisions are made collectively based on the stake weighted votes.

## How it Works

Validators can participate in the voting process by calling the `vote` function, specifying the amount of stake they wish to commit to a "yes" vote. The contract aggregates these votes, and if the total stake voting "yes" exceeds two-thirds (2/3) of the total active stake at any given moment, the voting process concludes.

Once a vote is finalized, the contract enters an immutable state, preventing any further modifications to its parameters or additional votes. This ensures the integrity and finality of the voting outcome.

## Key Features

*   **Stake-Weighted Voting**: Influence of a vote is directly proportional to the validator's stake.
*   **Decentralized Decision-Making**: Empowers validators to collectively govern critical contract functionalities.
*   **Immutability Post-Vote**: Guarantees that once a decision is reached, the contract's state related to that vote cannot be altered.
*   **Threshold-Based Consensus**: Requires a supermajority (2/3) of stake to pass a vote, ensuring robust consensus.
