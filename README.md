# armorCache

armorCache is a python tool dedicated to pulling market values off of TornCity's item market using API calls to determine profitability in regards to opening armor caches.

Armor Caches are a type of lootbox where a random drop will be rolled each time you open one. It is assumed to be I.I.D. and odds for each pull are published https://www.torn.com/rules.php#tab=odds_disclosure

The objective is to determine the Expected Value of a singular armor cache and to simulate long term behavior and whether or not it can be economically viable to open armor caches at a given price of the cache itself and the prices of the potential outcomes.

The gambler's ruin is also applied to determine how likely it is to attain a target cash value or go bankrupt.

### Notes and limitations: 

There are a select amount of items where the best way to sell them is to convert them into "Bunker Bucks" by exchanging it with the NPC shop. These items are manually selected due to their overall poor quality but this list is subject to change should a shift in their viability occur (but is extremely unlikely). The value of an individual "Bunker Buck" is calculated automatically and assumes the user trades their "Bucnker Bucks" optimally.

In addition, each individual armor rolls a random value for the bonus% and armor%. A high bonus% and armor% roll will sell far beyond the lowest price, however the rates of these are unknown so we assume a worst case scenario of the worst bonus and armor % so the armor is sold at the lowest market price. 
