# Risk Buster Demo

Neo fund holds 5 portfolios;
- ABORIGINAL AND TORRES STRAIT ISLANDER LAND AND SEA NEO FUND
- DISASTER READY FUND
- FUTURE FUND
- MEDICAL RESEARCH FUTURE FUND
- FUTURE DROUGHT FUND

Business problem statement: "As an investment/Compliance analyst, I want to find an efficient way to identify potential risks in our portfolios."

## Demo scripts

### Insight 1. Find all the relevant information about a company we invest.

1. In Bloom, ask a question; "Show me TATA MOTORS LTD. overview"

2. Expand on IS_SIMILAR_TO(Full text index score) relationship (siloed DB, 3rd party vendor DB, open source DB) → Exclusion info from open source data

3. “Is there any insights from reports?” → Competitor insights (TESLA, VOLKSWAGEN) and more

4. Explain how all connected data is represented in one scene easily

### Insight 2. Do we invest in companies others excluding from their portfolios for Climate issue?

While Neo Fund doesn't exclude any companies from their portfolio for climate issue, it is becoming more important. It is in our best interest to start considering this when making decisions and identify any high risk companies we currently invest.

1. In Bloom, ask a question; "Show me top 30 companies we invest that are DIRECTLY excluded by other funds for Climate"

2. Run degree centrality algorithm to highlight high risk companies

3. "Is there any insights from reports?" → Conocophilips, Devon energy insights

4. Take aways: 
    - Reduce investment in Conocophilips and monitor its competitor Occidental Petroleum
    - Keep a close eye on Devon energy as it's making a strategic move on environmental issue

### Insight 3. Do we invest in companies whose subsidiaries or parent companies are involved in dealing weapons?

Neo Fund excludes companies that deals weapon but it could be challenging to identify companies that are indirectly involved. GraphDB could easily explore complex relationships like this and help us identify potential risks that would've gone unnoticed otherwise.

1. In Bloom, ask a question; "Show me top 10 companies we invest that are INDIRECTLY excluded by other funds for Weapons"

2. "Show me the DIRECT exclusion connection" → China construction bank, Dongfeng motor group are high risk companies

3. Expand on countries/industries for further insight

