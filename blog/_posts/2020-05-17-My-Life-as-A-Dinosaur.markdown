---
layout: post
title:  "Evolution Path to Decentralized ASICs"
date:   2020-03-11 
excerpt_separator: <!--more-->
---
The news about ASICs for Nervos CKB came out recently, as the time of writing, there are four ASICs announced, the Toddminer C1, Toddminer C1 Pro, Bitmain K5 and PA miner — the first batch of C1 was delivered on March 9, K5 and PA Miner are expected to be delivered in April and C1 Pro in May.

Since mainnet launch, the total hashrate on CKB mainnet has been around 200TH/S on average, it is now gradually picking up (at the time of writing at ~500TH/S) with ASICs. Toddminer says C1+C1 Pro will provide 4,000TH/S, and it expects the total hashrate in mid-April will be 7,000–9,000TH/S.

People are surprised to see the rapid emergence of those CKB ASICs, especially given CKB uses a new design of hash function called the Eaglesong.

We have seen bitcoin and other PoW chains go through the mining phases of CPU-GPU-FPGA then finally ASICs. It’s taken four months for CKB ASICs to appear since its mainnet Lina in November, compared to four years for the first Bitcoin ASIC post-network launch. 

Things happen faster, but not necessarily any easier today compared with ten years ago, the evolution path to ASICs requires elaborate design in the environment today. 


Bad, good and inevitable
“ASIC? Is it good or bad?” — this is the first question people raised upon the news, and the answer to this question could vary, depending on where you are standing.

Mining is a zero-sum game, the issuance schedule of the coins is fixed and changing total miner hash power does not change how many coins are created over a certain time period. Each update of mining equipment usually leads to a great increase in hashrate and the rigs used in the previous phase will fade out as they are no longer profitable to operate.

There are different mining communities that support each approach, pro-ASIC or anti-ASIC; these views can polarize these communities so it is probably good to be conscious of this. 

Nervos is one of a few new layer 1 blockchains that puts faith in PoW as a mechanism to spur decentralization and provide long-term security. Some of the thinking on why it chose PoW over PoS and why it decided to use a new hash functionis captured in its positioning paper.

For a PoW blockchain network itself, the most important consideration is security. Coins at the greatest risk of 51% attack are the ones where there exist large amounts of hash power not actively mining that coin.

CPU, GPU and FPGA are general-purpose hardware that can mine other coins after conducting a 51% attack on your chain out of their own interest.

Let’s think about a scenario, someone malicious with a lot of general-purpose hash power could mine your coin “X” and send them to exchange to cash out for BTC and they can then conduct a 51% attack to re-organize the chain, returning the deposited coin “X” to themselves. The only calculation they need to make is: the BTC they gained > the electricity cost and the opportunity cost of mining other coins during the attack period.

What would be the case if the network was however mined by ASICs? We can look at Nervos for an example: at the time of writing, CKB trades at $0.006 with a market cap of 82M. The lifetime mining rewards total 33.6 billion CKB, which at the current price is around $25.2M per year in the first four years (4.2 billion CKB per year at $0.006/CKB).

Let’s say an attacker with 51% of hash power decided to attack CKB. If the attack depresses the price by 30% (a conservative guess for a new chain), the attacker would lose a substantial amount of future profit (~60M at $0.006/CKB) from their hardware purchase. This is the opportunity cost of their attack and gives us an idea of how much an attacker has to be able to gain from an attack just to break even with their costs (this does not yet include the ability for the other 49% of hash power to push back, or in the case of some chains, the ability of the core devs to change the hash algorithm).

That’s the reason why there is no ASIC mined coin (the ASIC could only mine one coin) that has ever been hit by a 51% attack. ASICs bring something that CPU/GPU/FPGA mining can’t offer: loyalty — with more “skin in the game”, the ASIC miners are incentivized to consider the long term success of the PoW chain.

“What if the ASIC miners dump the coins since the ASICs are more profitable than FPGAs -their cost per coin must be cheaper than GPU/FPGA miners right?”

Nah, the dynamics behind ASICs are powerful too.

For miners, the ASICs are much more expensive rigs than GPU/FPGAs, the payback cycle (回本周期) of an ASIC depends on the coin price, the total hashrate on the network and the price of the rig, which at one year it could be regarded as a good investment.

If the coin price went down, the payback cycle of the ASICs will become longer and the rigs lose value too; if the coin price went to the moon, more ASICs will join the game and the mining difficulty adjustment and competition between miners will raise the cost again, which we have already seen in bitcoin mining.

Because of the initial investment to mine this single coin, the ASIC miners will suffer substantially if anyone dumps the coins. Actually the ASICs can only emerge if the miners buying them are comfortable in the first place that no single entity could dump and the ASIC manufacturers are confident enough to make the efforts to build and ship the rigs because they see the demand from miners.

By end of the day, I do believe ASICs are inevitable and the only practical way to drive ASICs away is to continuously manually change the hash algorithm, at the cost of losing the existing hash rate (security at risk) and creating an unhappy and fragmented community.

ASIC miners will become an important part of the Nervos ecosystem and they are forming a holder community for the CKB coin.

Decentralized ASICs: A Rare Situation
The decentralization of ASIC production is something that has been discussed and experimented with other new blockchains (e.g. Sia coin’s community ASIC). But we have not yet seen a successful case, most coins have ended up with a dominant ASIC manufacturer. 

CKB’s current situation with ASICs is unique.

At the time of writing, there are three makers in the market that have announced CKB ASICs: Bitmain, Toddminer and PA miner — the latter two are small ASIC manufacturers, and if you check the spec of those ASICs, Toddminer’s C1 even has some timing and technical advantage — they use 28nm rather than Bitmain K5’s 40nm and delivered a month earlier than Bitmain.

Below are the key factors that I think have contributed to the decentralization of CKB ASICs production:

A new and simple PoW hash function Eaglesong - which significantly lowers the barrier and cost for hardware development

Enough mining pool support and traction from investors - so the ASIC makers are comfortable taking the risk

ASIC-neutral — the core dev team says it does not participate in ASIC manufacturing nor will it change the hash function to avoid ASICs (and people trust their words)

The initial investment in making a new ASIC is usually in the millions and it could vary from 1~2 million to 20 million or more, depending on what chips you are using, it is equivalent to a VC investment and not that friendly to small and new players.

The biggest ASIC manufacturers in China — Ebang, MicroBT, Innosilicon, Canaan Creative and Bitmain — are mostly focusing on BTC, which generates an annual return of over $5 billion in mining rewards and transaction fees as of March 9, 2020.

CKB is a much smaller pie, the mining rewards are currently $25.2M per year in the first four years (4.2 billion CKB per year at $0.006/CKB as of March 9 2020), but its new and simple hash algorithm makes CKB ASIC design a low-hanging fruit, and the first mover will get a bigger piece of the rewards than their competitors.

The Nervos foundation has dedicated a lot of effort in building its mining communities. It started mining competition on testnet last May and by the time of mainnet launch in November, it had over ten mining pools support and GPU mixed with FPGA mining.

Most importantly, the core devs take a neutral position toward ASICs, which creates space for an efficient market to grow, and we saw competition came out. 


Typically, stakeholders of a layer 1 blockchain are core devs, miners, builders/creators (in the ecosystem) and coin holders/buyers. They are strongly coupled in a growing PoW ecosystem.

Miners maintain the network and get paid through mining rewards (new coins supplier)

Core devs maintain the protocol and are responsible for further upgrades

Builders/creators create applications and draw new users into the ecosystem

Coin holders/buyers is a broader category that may include the three above. They drive the demand for the tokens

The ASIC manufacturers are optimistic about the project’s future (token price) and trying to establish a business in selling rigs to CKB miners, what would make them most nervous is the possibility of the core devs changing the hash algorithm after they have already manufactured ASICs. This would make the rigs worthless, thus the ASIC-neutral message from the CKB core-dev team is very important and encouraging for ASIC makers, especially the smaller players.

Will CKB eventually have a dominating ASIC?

Eventually? I don’t know. Any ASIC manufacturer could jump in and uses a 7nm chip to make a CKB ASIC and sell the rigs at a current average price of other existing ASICs, it probably will be dominating. However, the initial investment probably will be over 20 million, not counting existing and potential competition. It’s unlikely for a rational player to do so at the current token price/block rewards. ASIC manufacture is a competitive and risky business, especially for new players.

Did Nervos Foundation funded ASIC production or participate in mining? 

I don’t think this is a valid suspicion from an economic perspective.

The Nervos Foundation already did a private and public sale for token distribution, and the core dev/builders/creators have been and will be funded by the token sale raise that are under the custody of a foundation - This so-called “pre-mine” portion is 25% less than the total mining rewards according to Nervos’ token distribution.

Considering this, what would be the incentive for the foundation to fund ASIC production — mining rewards itself is a bounty of ~200M in total and ~$25M per year to start with — why would the foundation want to spend more on this for miners to get coins at an even cheaper cost? 

There is no incentive for the foundation to even participate in mining, given its ultimate goal is decentralization with a broader distribution of the tokens, otherwise it should have chosen PoS over PoW for its convenience.

As CKB has now moved into the era of ASICs, it has a substantial lead in terms of security, immutability and censorship resistance than any PoW chains that do not have ASICs. 

My only wish for her is to live long and prosper.


Relevant readings

A brief history of bitcoin mining hardware

Crypto Mining 101 — Overview & Landscape of the Mining Industry

How Coinbase views proof of work security

In support of the proof of work [un]fair launch

No, Concentration Among Miners Isn’t Going to Break Bitcoin

Is The War Against ASICs Worth Fighting?

It’s the settlement assurances, stupid

Thanks DC, Matt Quinn, Jan Xie and Derek Hsue for providing feedback to the article.

Disclaimer: Not investment advice and any views expressed are personal and do not represent an official position of the Nervos project.
