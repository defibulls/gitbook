# BULLION



Each TR Bull NFT (Normal or Alpha) accrues a specific amount of Bullion monthly. The amount of TR Bull accrues is derived from the cost of the NFT multiplied by the Magnifier value. Accrued Bullion serves two primary purposes within The Ranches Ecosystem:

* Reward Distribution.
* Voting Power.

| Type of TR Bull           | Cost | Magnifier | Accrued Bullion  |
| ------------------------- | :--: | :-------: | :--------------: |
| Regular TR Bull           |  180 |    100    |      18,000      |
| Regular TR Bull w/ Turtle |  180 |    225    |      40,500      |
| Bronze Alpha TR Bull      |  350 |    125    |      43,750      |
| Regular TR Bull w/ Frog   |  180 |    700    |      126,000     |
| Silver Alpha TR Bull      | 1000 |    150    |      150,000     |
| Gold Alpha TR Bull        | 5000 |    200    |     1,000,000    |



## Understanding Bullion:&#x20;

* Bullion itself does not have a fixed value. Instead, it serves as a basis for calculating the percentage of rewards each stakeholder receives based on their staked amount and voting activity.
* At the start of each month, the smart contract computes the total bullion accumulated by the staked owner across all NFTs they possess. This process captures a snapshot of the owner's holdings, which can be used to leverage their bullion within the ecosystem. Essentially, bullion serves as a means of tracking ownership and enabling participation in the system.
* Before distributing rewards to stakeholders, the bullion is deliberately calculated to determine the reward allocation ratio for that month's reward tokens. This means that, for instance, if five investments/projects are rewarded with five distinct ERC20 tokens, the reward ratio for each stakeholder remains consistent across all tokens until the entire reward distribution process is concluded.
* After rewards are dispensed, all bullion is wiped from stakeholders' accounts and recalculated the following month to repeat the rewarding process. Regardless of which NFT you stake, the bullion output remains the same. The crucial reward eligibility requirement is to stake at least one NFT.
* Bullion is only calculated for NFTs owned by the staked NFTs owner's address. Any NFT held on a marketplace transferred to another wallet is not calculated on your behalf. Distributing NFTs across multiple wallets does not impact the cumulative bullion earned compared to storing them in a single wallet.
* At the beginning of each month, bullion is computed, and by the 10th, stakeholders receive their rewards. This ensures that they have sufficient bullion available to participate in marketplace activities, such as wagering on bull runs and contests, that involve the transfer of bullion among them. These activities can be performed before reward distribution. By following this approach, even if someone owns just one Normal TR Bull, they can participate in such activities and potentially increase their monthly earnings by 10x, 100x, or even 1000x, giving them a chance to earn higher rewards.
* Once all NFTs are sold, the total supply of bullion is capped at 106,600,000, and there are no means to increase an owner's bullion value other than the computed value of their NFTs. Any additional bullion earned through Bull Battles has a net zero effect since it is transferred from one NFT owner to another and not created out of thin air. As a result, the bullion value is not inflationary and remains stable.
