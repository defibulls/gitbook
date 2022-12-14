# HOSTING

## HOSTING FEES FOR THE BTC Bulls

What is this, and why is this important? Let's play out an example of how this project will go. We start the project and sell our BTC Bull NFTs, and purchase miners. We go through the first three tiers and sell 2999 BTC Bulls. 89% of the minting cost would be buying BTC miners for the project.&#x20;

* TIER 1 = (999 \* 350) \* 0.89&#x20;
* TIER 2 = (1000 \* 360) \* 0.89&#x20;
* TIER 3 = (1000 \* 370) \* 0.89&#x20;

BTC MINERS SAFE == ((999 \* 350) + (1000 \* 360) + (1000 \* 370 )) \* 0.89  ==  $960,888.50

The BTC MINERS SAFE is then used to purchase and build the project's BTC MINER CLUSTER. Let's assume we can purchase 100 TH/s Antminer S19s for ≈$4000 each.

$960,888.50 / $4000 == ≈ 240 Antminer S19 100Th/s&#x20;

When factoring in tax or other transaction expenses, the BTC MINER CLUSTER starts with about 240 s19j Pro miners or about 24,000 TH/s of mining power.&#x20;

<figure><img src="../../../.gitbook/assets/Farm (2).png" alt=""><figcaption></figcaption></figure>

As an owner of a BTC Bull(s), you are leasing the fenced plot of land, a stockyard, for your Bulls to live and graze. Some owners will have stockyards with a single Bull, while others can create much larger ones. There is no limit on how many BTC Bulls can be housed within a particular stockyard. Each BTC Bull within your designated plot carries a max $15 hosting fee per month. The collection of individual stockyard hosting fees goes directly to pay for the actual hosting fees of the BTC Bulls mining cluster at Compass Mining.&#x20;

This approach allows each BTC Bull within The Ranch to share the hosting invoice evenly. In the above example, 240 miners on the invoice would be ≈ $38,000 if we average a $156.60 hosting fee per miner. Since we have 2999 BTC Bulls in circulation, each BTC Bull NFT will share that invoice, and that calculation would come out to be $12.67 per BTC Bull. For the sake of easy math and never wanting to be short on the project, we will round up each hosting calculation. In this example, we would set the monthly hosting fee to $13 and would be able to retain a small amount left over in our HOSTING SAFE wallet that would go to pay next month to pay on later hosting invoices. The intent behind this approach is to avoid having excess hosting fees sitting in a wallet for no reason. Unlike other projects, our hosting fees serve the direct purpose of paying the actual invoices from Compass Mining, not trying to build any treasury for the project. &#x20;

Through compounding efforts, our BTC Mining Cluster has the potential to grow very large and powerful. The following month we could add more miners as more Tiers sell out and our compounding efforts start. This could give us an invoice of $185,000 shared between all 9960\* BTC Bulls. With the set hosting fees for each plot, once we collected the $15 from each BTC Bull, as that is the max hosting fee allowed for each BTC Bull on the project, we would still be short of paying the monthly invoice.&#x20;

$185,000 - $149,400 == $30,600 left to cover&#x20;

In this instance, we would have to convert $30,600 of our mined BTC to pay the remainder of the invoice. The rest of that mined BTC gets dispersed as monthly rewards, according to FIG 0.&#x20;

From all our projections, the last thing we want to do as a BTC Bulls Community is burn our mined Bitcoin to pay for hosting invoices. However, there is a delicate line between burning Bitcoin for hosting fees and having reasonable and consistent hosting fee expectations for all BTC Bull NFT holders. &#x20;

&#x20;_\* 9960 comes from 20 BTC Bulls exempt from Minting Luck, + we will rotate 20 other BTC Bulls every three months (January, April, July, and October) via a drawing; these NFTs are exempt from hosting fees._&#x20;

#### THE HOSTING SAFE

A fundamental concept and design feature of the project revolves around the HOSTING\_SAFE and ensuring we keep funds in there to keep the project healthy. Every plot owner must pay the hosting fee for all their BTC Bulls on the property. Every plot/stockyard owner within The Ranch has a 'Hosting Clock' on their account ranging from 0-3. This represents how many monthly reward periods can go by before The Ranch queries your stockyard account. The Ranch only queries accounts whenever a plot owner's account reaches zero on their hosting clock. &#x20;

Essentially each plot owners accounts looks like this:&#x20;

<figure><img src="../../../.gitbook/assets/image (1) (8).png" alt=""><figcaption><p>FIG_ACCOUNT</p></figcaption></figure>

When a plot owner's stockyard is checked, we check to see if the plot owner has WBTC rewards in their account. If any account does, we then check if that account has a hostingFeeBalance greater than zero. If they have a hosting balance greater than zero, we check to see if the user's hosting fee reserve balance is larger than their hosting fee balance. If that is the case, we will auto-pay the hosting fee balance for that plot owner's account using their hosting reserve balance and reset their hosting fee balance to 0 and their HostingClock to 3. If the account hosting reserve balance can not cover the hosting fee balance, we are forced to settle up with the account in another way. We would take the WBTC in that owner's account and send it to the HOSTING SAFE multi-sig wallet and then reset that account's hosting fee balance and set the hosting clock to 3. Essentially we are liquidating the WBTC from that user's account and will have to sell it to help pay for the community hosting fee invoices at the mining facility. That plots owners account also has a counter that keeps track of how many times they have been liquidated, which will be incremented by 1.  The process flow looks like this:

<figure><img src="../../../.gitbook/assets/image (9) (2).png" alt=""><figcaption><p>FIG 4</p></figcaption></figure>

The Hosting Clock automates our contract to do an 'auto-pay' feature to pay account hosting fees. Users always have the option to pay for the hosting fees manually before their hosting clock gets to zero if they wish. The manual transaction to pay hosting fees follows the logic in the following figure. If a user has enough USDC.e within their hosting fee reserve balance, the hosting fee balance will be deducted from that balance. Otherwise, the user will need to pay the hosting fees from their wallet using USDC. A successful transaction sends funds to the Hosting Safe and resets the account hosting fee balance to zero and hostingClock back to three.

<figure><img src="../../../.gitbook/assets/image (5) (4).png" alt=""><figcaption><p>FIG 5</p></figcaption></figure>

The key difference between our liquidation structure and other projects, such as StrongBlock, is if a user gets behind and doesn't pay their hosting fees. They wouldn't lose everything as you would have in StrongBlock. In our ecosystem, the user only forfeits the current WBTC in their account on our contract, and then they are reset back to good standing, ready to receive next month's WBTC rewards. &#x20;

#### FUNDING YOUR HOSTING RESERVE BALANCE

Within the project, we have built many ways a user can increase their USDC.e balances on the contract and will continue to build more as time goes on. Referring people to the project gives you 2% of their minting transaction cost. The Minting Giveaway and the Royalty Giveaway will do the same and can fund an account for a long time. To transfer funds from an account's USDC.e rewards balance to their hosting reserve balance, users must send their rewards to their wallet and fund the hosting reserve directly. &#x20;

To fund your hosting reserve balance to cover auto-pay events, you do this in the hosting section of your account.  This allows users always to have USDC.e in their account to pay for hosting fees and avoid liquidation. As long as the user has more in their hosting reserve balance than in their hosting fee balance, they can't get liquidated. Users can deposit up to $1000 per transaction into their hosting reserve balance, protecting them from liquidation as far as the user wants to project it out into the future. All funds within the hosting reserve for an account can be withdrawn at any time.&#x20;



## HOSTING FEES FOR THE BTC Bears

The BTC Bears work exactly like the BTC Bulls, with one exception. Firstly, the amount of hosting fees due from each BTC Bear is only a max of $5 per month, whereas the BTC Bulls carry a $15 monthly max obligation.&#x20;

The hosting difference stems from what needs to happen on The Ranch regarding both animals. The BTC Bulls are domesticated cattle that are provided land for grazing, shelter, and food. The BTC Bears, on the other hand, live in the surrounding forest of the property and thus don't incur the same expense on our property other than fencing and general preying protection from attacking our livestock.&#x20;

To desire to own BTC Bulls or BTC Bears depends on your mathematical stance on their actions and what they are doing for their community. Playing out the same scenario as the BTC Bulls did would look like this:

The BTC Bears Community Mining cluster also has 240 miners getting the same electricity rate; each BTC Bear would contribute to the hosting fee evenly. Working with an invoice of ≈$38,000 and having 2999 BTC Bears in circulation, we would only be able to contribute ≈$15,000 towards that invoice.

$38,000 - $15,000 == ≈$23,00 left to cover&#x20;

In this instance, we would have to convert ≈$23,000  of our mined BTC to pay the remainder of the invoice. The rest of that mined BTC gets dispersed as monthly rewards to the Bears Community, according to FIG 0.&#x20;

The BTC Bears do everything else under the same rules as the BTC Bulls regarding Minting Giveaways, Royalty Giveaways, and liquidation events.



## WHEN DO HOSTING FEES START?

Hosting Fees pay the invoices at Compass Mining. Thus, they won't start until an invoice is generated, which would be on the first award event estimated for Q1 of 2023.



## WEBSITE UNDERSTANDING:

### **Hosting Reserve deposit and withdrawal:**&#x20;

<figure><img src="../../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>

The "+" in the hosting reserve balance section is to deposit USDC.e into your hosting reserve balance. Each transaction can be up to $1000.&#x20;

The "-" would withdraw your entire hosting reserve balance.



### **Hosting Clock:**&#x20;

<figure><img src="../../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

&#x20;__&#x20;

A three indicates the clock is full, and the account won't be checked for a liquidation event for three more reward cycles (1st-5th of each month). 2 would indicate that 1 reward cycle has happened since the last time paid their hosting invoice balance. This will always be a number between 1 to 3 on the website. &#x20;







<figure><img src="../../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

**A**: shows how many NFTs you own in this particular community.&#x20;

**B**: The hosting invoice balance is the hosting fees for this particular owner. 4 NFTs, and the hosting clock was deducted by 1 (starts at 3). &#x20;

**C**: The Hosting Reserve Balance is the amount of money deposited into the owner's account to cover the hosting invoice balance when this owner's account gets to zero.

Is the owner of these NFTs safe from being liquidated when their hosting clock gets to zero?  No, because this account doesn't have enough in its reserve balance to cover the hosting invoice when their hosting clock gets to zero.&#x20;

* the current position is two on the hosting clock, $100 in reserve, and $60 on their hosting invoice balance.&#x20;
* next pay period would be one on the hosting clock, $100 in reserve, and $120 on their hosting invoice balance.&#x20;
* next pay period would be 0 on the hosting clock, $100 in reserve, and $180 on their hosting invoice balance.&#x20;
  * At a hosting clock of zero, we check the account and check if they have more in their reserve than their hosting invoice balance. No, thus, liquidation would happen here as their WBTC rewards would be transferred to the hosting wallet to help pay for hosting invoices for the community.&#x20;



Now I will add $100 to the hosting reserve balance:&#x20;

<figure><img src="../../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

The shield represents how many times the hosting clock for this owner could get to zero and auto-pay for their hosting invoice balance. The shield of '1' means the account will be safe for one liquidation check.&#x20;

* the current position is two on the hosting clock, $200 in reserve, and $60 on their hosting invoice balance.&#x20;
* next reward cycle would decrease the hosting clock to one, $200 in reserve, and $120 on their hosting invoice balance.&#x20;
* next reward cycle would decrease the hosting clock to zero, $200 in reserve, and $180 on their hosting invoice balance.&#x20;
  * Now that the hosting clock gets to zero, the account is checked and does have enough in the hosting reserve to cover the hosting invoice balance and an auto-pay happens. The hosting clock is reset to 3, the hosting invoice balance is set to zero and the hosting reserve balance is decreased by $180



