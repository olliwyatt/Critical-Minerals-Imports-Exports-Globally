**Critical Minerals Trade: 1995–2024**

**Project Overview**

This project investigates international trade in critical minerals, focusing on cobalt, lithium, and rare-earth products between 1995 and 2024.

The project uses R to retrieve, organize, and validate historical trade data from the United Nations Comtrade database. Further analysis will examine changes in critical-mineral trade patterns and their relationships with economic development and governance.

**Data Collection**

Trade data were retrieved from the UN Comtrade API using the comtradr package in R. A reusable function was developed to automate data retrieval across commodity codes and five-year intervals, cache API responses locally, and consolidate the resulting records into a single dataset.

The resulting dataset contains 25,051 observations across seven cobalt, lithium, and rare-earth product categories covering 1995–2024.

The data include country-level reported imports and exports with the world as the aggregate trading partner, rather than bilateral trade flows between individual countries.

Historical commodity classification changes were examined, with earlier cobalt product classifications documented separately.

**Repository**

Critical Minerals API Dataset.qmd: Contains the R code used to call the UN Comtrade API, define commodity categories, construct datasets, and perform initial validation checks.

mineral_trade_1995_2024.csv: Main dataset containing 25,051 trade observations.

cobalt_historical_1995_2001.csv: Historical cobalt trade records for HS code 810510, stored separately because this classification includes products not covered by the later HS code 810520.


**Data Source**

United Nations Statistics Division, UN Comtrade Database.

https://comtradeplus.un.org/

