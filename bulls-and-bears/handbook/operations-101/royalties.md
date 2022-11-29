# ROYALTIES

## ![](<../../../.gitbook/assets/image (1) (5) (2).png>)ROYALTY KICKBACKS

<figure><img src="../../../.gitbook/assets/image (3) (1) (5).png" alt=""><figcaption></figcaption></figure>

Also uses Chainlinks VRFv2 functionality.&#x20;

* What is VRF?  Chainlink VRF (Verifiable Random Function) is a provably fair and verifiable random number generator (RNG) that enables smart contracts to access random values.

#### ROYALTY RAFFLE

There will be a 12.5% royalty fee when selling BTC Bulls on OpenSea.  2.5% gets paid to OpenSea as a fee, and the remaining 10% is split 50/50.&#x20;

* **50%** going back to The Ranch for project development and project-related costs.&#x20;
* **50%** goes into our monthly Royalty Raffle. Each month, this 50% will be divided equally and dispersed between up to 3 BTC Bull owners. This amount will be uploaded into the USDC.e rewards balance on the contract for those winning BTC Bull owners. See the raffle explanation for a deeper explanation, further explanation [here](royalties.md). &#x20;

Our community will be filled with holders with long-term mindsets, but there will always be those who need to sell for liquidity and/or profit opportunities. Looking at what other projects have done in the past, if we get anywhere close to a quarter of the numbers those projects hit, these raffle amounts have the potential to be special.

To win a royalty raffle, the BTC Bull owner's address must be free of any liquidations. If a BTC Bull owner is chosen as the winner but does have liquidations, the function will skip that address and move on to the index number in the queue.&#x20;

As previously stated, there is a 12.5% royalty when selling BTC Bulls on OpenSea. 50% of the Royalty disbursement will be raffled off using the Royalty Raffle Contract. Only BTC Bull owners that have not been liquidated before will be eligible to win the Royalty Raffle. This is the best way to thank participants who stay on top of their game, which helps our ecosystem.&#x20;

### The way the function works:&#x20;

We will request 20 very large random numbers using chainlinks VRF setup.&#x20;

These numbers go through a few mathematical functions to arrive at 20 possible NFT indexes that are eligible to win the USDC.e balance on the Royalty Raffle contract (50% of that month's Royalties)

Let's assume we have found the twenty winning indexes; 5, 55, 83, 189, 788, 4422, 8832, and so on.&#x20;

* First, we check who owns index number 5 and get the owner
* Secondly, check if that address has been liquidated before. If they haven't, we place them in the winning array. If they have, we skip them and move on to the following number in the list, which is 55.&#x20;
* This process continues until we find three winners that meet the criteria of winning (owner of that NFT and no liquidations on account).&#x20;
* Once we find three winners, the function ends. We split the balance into three equal parts and award the three winners.&#x20;
* If only one person of the 20 index numbers meets the eligibility criteria. That single address will receive the entire balance (being 3x larger).&#x20;
* If no one meets the criteria in the 20 winning numbers, we repeat the process until someone wins.&#x20;

