# Methodology 
 
## 1. Our philosophy
 
 
**Unambiguity**. When identifying clusters, we asked ourselves: could a random wallet end up in this cluster? Could such a coincidence happen in parallel universes? Thus, we identified a cluster only if the answer was unequivocally no. We clearly understand that even one unfairly excluded user negates the benefit of thousands of fairly excluded ones.
 
**Representativeness and Transparency**. In describing any cluster, we followed the rule that the content of the report should make it immediately clear and unambiguous why this group of wallets was reported. Even someone without a significant background in Web3 should be able to easily understand the report.
 
**Combination of Methods**. We respect both mathematical methods based on big data and manual review. However, we understand that without each other, they can make serious mistakes. For example, you might devise perfect search criteria, but without careful manual processing, they do not guarantee reliability. This is why we use comprehensive verification based on a symbiosis of these methods
 
**Clustering as the Ultimate Solution**. Any other solutions are meaningless as it is crucial to distinctly differentiate between farmers and Sybils. In our view, methods other than clustering do not allow for a clear demarcation, with the primary focus of the search needing to be solely around Sybils. The boundary between a farmer and a legitimate wallet is quite difficult to draw in the current realities (e.g., should people like Justin Sun be deprived of airdrops?)
 
**Distributed Expertise**. From the report, it is evident that our team is highly distributed, consisting of specialized mathematicians, developers, and data analysts. This diversity allows us to conduct cross-checks and avoid errors common to solo investigators. The strength lies in decentralization!
 
 
## 2. “Similarities” - methodology
________________________________________________________________________________  
TL;DR, but highly recommended to read full version after
 
1. Collect data from the provided dataset, Dune Analytics, and raw blockchain data to enrich the table and determine values for 10+ parameters.
 
2. Select a set of 3-4 criteria from the 10 available criteria that must be identical.
 
3. Obtain raw data. Manually and machine-process each cluster in search of additional similar parameters.
 
4. In some cases, for additional verification, process a large dataset with common on-chain patterns (carefully filtering out noise, such as multisend shitcoins).
 
5. Create a markdown table for each class for clarity and obviousness of similar data.
_____________________________________________________________________________________________________________
In our methodology, we drew inspiration from the filtering philosophy employed by ZigZag. They utilized an approach based on the complete convergence of multiple methods.
We decided to expand on their approach by using more than 10 different criteria. These included both fairly obvious metrics such as the number of transactions, the number of source and destination chains, and some innovative solutions like the highest volume of a single transaction and the specific day on which such a transaction occurred.
This method, for example, serving as our primary key, allows us to identify Sybils who artificially wash-traded volume on a specific day using a single amount and then simply updated the parameter for the number of active days/weeks/months.
As mentioned earlier, we did not allow for random errors. Thus, we clustered wallets only when, after merging by "primary parameters," we observed unequivocal similarity in other parameters.
 
Through this process, we identified groups that met the following criteria (example):
 
`-Consisting of more than 20 wallets.`  
`-Having the same (to the nearest whole number) maximum volume for a single transaction.`  
`-The max volume transaction occurred on the same day.`  
`-The first transaction in L0 was conducted on the same day with a margin of 2 days (e.g., January 10-12, 2023).`  
`-The first transaction on the chain overall was conducted within a margin of 2 days (e.g., January 1-3, 2023).`  
`-The number of source chains used varied from 7 to 8.`  

Despite the obviousness of some situations, we adhered to the presumption of innocence and the presumption of proof (returning to the philosophy and rule of unambiguity). In cases where the argumentation was lacking even 0.01% to reach 100% certainty, we decided to additionally export all common protocols with which the wallets in the cluster interacted Most "exemplary" protocols were selected. For example, it is rather "strange" that 26! wallets had interaction with one particular CEX, had the same wallet birthday, all conducted transactions with 7 identical source chains and had a total volume from 11200$ to 11300$, and conducted the first $STG tx on exactly the same day too. However, it is even stranger that they all as one interacted with a number of DeFi protocols on Arbitrum, which have no token (and are difficult for a beginner), entered Persona raffle and yet are not involved in any basic DeFI layer, like Uniswap
 
We then meticulously manually processed this information and retained Sybil groups where a common behavioral pattern was clearly traceable.
 
Thus, each of the clusters we proposed can unequivocally be considered to consist of Sybils from the same group. To prove this, we provide a table of similarity metrics for each group of Sybils.
 
Additionally, we emphasize that all data can be re-verified and confirmed on your end
 
Link to code will be provided after bounty closure
 
 
