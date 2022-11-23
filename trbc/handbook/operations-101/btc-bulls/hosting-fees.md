# HOSTING FEES

<figure><img src="../../../../.gitbook/assets/image (1) (3).png" alt=""><figcaption></figcaption></figure>

A hypothetical example outlines how this works for two users, Star and Triangle.

Both buy a BTC Bull in the middle of January. The key difference is that Triangle has $100 in their USDC.e rewards balance. That could have come from a raffle or referral rewards, or they uploaded $100 into their USDC.e rewards balance themselves. &#x20;

Rewards for the month will always happen between the 1st and 5th of the month. Both users were rewarded in February, and their accounts were updated accordingly.  Each user received .01 WBTC and had their maintenance clock decremented by one, and the maintenance balance increased by $15. &#x20;

Both get rewarded in March, as expected.&#x20;

The difference happens in April at the purple circle icon location. Both users were processed for the month and checked for liquidation because they had their maintenance clock decremented by 1, equaling 0.

* Triangle had more than $45 in their USDC.e reward balance, which was used to automatically pay the maintenance fee and reset their maintenance variables while avoiding liquidation and keeping all WBTC earned.  &#x20;
* Star did not have $45 in their USDC.e reward balance and thus got liquidated, transferring the WBTC out of their account and sending it to the HOSTING SAFE wallet to help pay monthly hosting invoices. Maintenance variables were also reset for Star, but the liquidation count did increment\*.&#x20;

The liquidation count does not affect how much WBTC is received in the future. All BTC Bulls will be awarded the same throughout the project. The liquidation count is only being used for the Royalty Raffle; only users that have NOT been liquidated are eligible to win.&#x20;

