# ROYALTIES

## ![](<../../../.gitbook/assets/image (1) (5) (2).png>)ROYALTY SWEEPSTAKES

<figure><img src="../../../.gitbook/assets/image (3) (1) (5).png" alt=""><figcaption></figcaption></figure>

Also uses Chainlinks VRFv2 functionality.&#x20;

* What is VRF?  Chainlink VRF (Verifiable Random Function) is a provably fair and verifiable random number generator (RNG) that enables smart contracts to access random values.

#### ROYALTY RAFFLE

There will be a 12.5% royalty fee when selling BTC Bulls on OpenSea.  2.5% gets paid to OpenSea as a fee, and the remaining 10% is split 50/50.&#x20;

* **50%** going back to The Ranch for project development and project-related costs.&#x20;
* **50%** goes into our monthly Royalty Raffle. Each month, this 50% will be divided equally and dispersed between up to 3 BTC Bull owners. This amount will be uploaded into the USDC.e rewards balance on the contract for those winning BTC Bull owners. See the raffle explanation for a deeper explanation, further explanation [here](royalties.md). &#x20;

Our community will be filled with holders with long-term mindsets, but there will always be those who need to sell for liquidity and/or profit opportunities. Looking at what other projects have done in the past, if we get anywhere close to a quarter of the numbers those projects hit, these raffle amounts have the potential to be special.

To win royalty sweepstakes, the BTC Bull owner's address must have a liquidation score of zero. If a BTC Bull owner is chosen as the winner but does have liquidations, the function will skip that address and move on to the index number in the queue. This is the best way to thank participants who stay on top of their game, which helps our ecosystem.&#x20;

### The way the function works:&#x20;

We first determine the amount of USDC that will be rewarded during this royalty sweepstakes and see how many times the $500 award max amount can be divided into it to find the number\_of\_winners.

If that number\_of\_winners is 5, then we will request ten more numbers than that from the Chainlink VRF system; 15 incredibly large numbers.&#x20;

If that number\_of\_winners is 18, then we will request double that amount from the Chainlink VRF system; 36 incredibly larger numbers. &#x20;

These numbers go through a few mathematical functions to arrive at possible NFT index numbers of the BTC Bulls or BTC Bears, depending on which contract is awarded.

For example, let's assume we needed to find three winners because we were giving away $1830, 3 winners would be getting $500 each, and $30 remains on the contract for the next royalty sweepstakes.

We received our list of numbers from the Chainlink VRF system and deduced those numbers into indexes of the potential winners. A list of potential winning indexes might be 5, 55, 83, 189, 788, 4422, 8832, and so on.

1. Check who owns index number 5 and get the owner's address.
2. Check if that address has a liquidation count of zero. If true, we place them in the winning array list. If they have a score of more than 0, we skip them and move on to the following number in the list, which is 55.&#x20;
3. This process continues until we find three winners that meet the winning criteria.&#x20;
4. Once we find three winners, the function ends.

We send the list of winners each $500, and the fun starts all over again next month.&#x20;



_Alternative Means of Entry (AMOE)_

* _No purchase Necessary_
* _For additional details, please visit the official discord channel "The Ranch Info / amoe"_

