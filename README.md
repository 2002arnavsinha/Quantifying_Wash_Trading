# Wash Trading in Opensea Marketplace

<img width="563" alt="image" src="https://github.com/user-attachments/assets/229d6fd0-4564-4aca-b408-6409207c495b" />

<img width="387" alt="image" src="https://github.com/user-attachments/assets/59c2f427-4adc-4365-9b13-f0512b9b1328" />


 Cycle detection identifies closed loops where an NFT returns to its original owner within a
 short period. These cycles are defined as sequences of up to four trades that occur within
 30 days, such as A to BtoAorAtoBtoCtoA.Fromthedataanalyzed, 2,381cycles were
 detected with a total trading volume of $8.42 million, an average of 3.25 trades per cycle,
 and a mean duration of 6.38 days. The presence of such loops strongly indicates potential
 wash trading, as the return to the original address suggests self-trading. Moreover, 637
 of these cycles, accounting for $2.78 million in volume, exhibited minimal price variation
 (below 0.05), a common sign of artificially inflated trade volumes while maintaining stable
 prices, a hallmark of wash trading behavior.
 
 Temporal clustering reveals rapid bursts of NFT trades exhibiting unusual price be
havior. These clusters are identified using DBSCAN clustering with a one-hour window,
 requiring more than ten trades per cluster, with price variances either below 0.05 (indi
cating stability) or above 100 (indicating extreme volatility). Additionally, seller overlap
 must exceed 50%, meaning fewer than half of the sellers are unique. The results indi
cate 745 such clusters with a total trade volume of $3.07 million and an average of 69.3
 trades per cluster, all characterized by extreme price variance. The short time frame of
 these trades, averaging 2.5 hours per cluster, along with the repetition of sellers, suggests
 coordinated activity. This high-frequency trading pattern, combined with extreme price
 movements, points to deliberate price manipulation rather than just volume boosting,
 making it a strong indicator of wash trading.
 
 Community detection focuses on identifying dense networks of addresses that engage
 in substantial internal trading. A detected community must include between 5 and 100
 addresses, execute more than 10 trades, have a trade volume exceeding $2,000, and main
tain a trade density above 2 (meaning each address is involved in multiple transactions).
 Additionally, the price variance within these communities must either be very low (below 1) or very high (above 50), and at least 30% of the sellers must be repeated participants.

The analysis uncovered 21 such communities, with a total volume of $1.11 million, an
 average of 11.19 addresses per community, and 30.71 trades. The high internal trade
 density and repeated sellers suggest coordinated activity, with low-variance communi
ties likely engaging in volume inflation and high-variance ones potentially manipulating
 prices. These characteristics strongly indicate collusion, further supporting the presence
 of wash trading within NFT markets. 
