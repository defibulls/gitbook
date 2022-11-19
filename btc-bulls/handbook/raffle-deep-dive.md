# RAFFLE DEEP DIVE

As stated in the OPERATIONS 101 section, there is a 10% royalty when selling BTC Bulls on the secondary Marketplace. This royalty money goes back to the creator of the NFTs, but the choice has been made to thank the people of The Ranch community for making this a great project.&#x20;

Each month 50% of the Royalty disbursement will be raffled off using the Royalty Raffle Contract. Only BTC Bull owners that have not been liquidated before will be eligible to win the royalty raffle. This is the best way to thank participants who stay on top of their own personal game, which helps our ecosystem.&#x20;

### The way the function works:&#x20;

We will request 20 very large random numbers using Chainlinks VRF setup.&#x20;

These numbers go through a few mathematical functions to arrive at 20 possible NFT indexes that are eligible to win the USDC.e balance on the Royalty Raffle contract (50% of that month's Royalties)

Let's assume we now have found the twenty winning indexes; 5, 55, 83, 189, 788, 4422, 8832, and so on.&#x20;

* Check who owns index number 5 and get the address owner
* Check if that address has been liquidated before. If they haven't, we place them in the winning array. If they have, we skip them and move on to the following number in the list, which is 55.&#x20;
* This process continues until we find three winners that meet the criteria of winning (owner of that NFT and no liquidations on account).&#x20;
* Once we find three winners, the function ends. We split the balance into three equal parts and award the three winners.&#x20;
* If only 1 person of the 20 index numbers meets the eligibility criteria. That single address will receive the entire balance (being 3x larger).&#x20;
* If no one meets the criteria in the 20 winning numbers, we repeat the process until someone wins.&#x20;

