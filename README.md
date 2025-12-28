## Portuguese Real Estate Market – Property Listings Analysis

This project provides an end-to-end analytical view of the Portuguese real estate market, focusing specifically on active property listings, rather than completed transactions. The dataset is updated weekly and represents the full supply of properties available for sale across Portugal, including apartments, houses, land, commercial spaces, garages, industrial properties, farms, and rural estates.

The objective of this analysis is to understand market structure, price dynamics, and spatial distribution of supply, offering insights into how different regions, property types, and typologies contribute to the overall real estate landscape.


## Project Purpose
The main purpose of this project was to build a start-to-end data analysis pipeline, replicating a real-world analytical workflow:

- Raw data ingestion and validation  
- Data quality assessment and treatment  
- Feature selection and transformation  
- Data enrichment with external indicators  
- Interactive dashboard development for exploratory analysis and decision support  

Rather than simply visualizing data, the project emphasizes data quality, analytical rigor, and business interpretation, ensuring that insights are both reliable and meaningful.


## Analytical Process

The analysis began with a detailed data quality assessment, including the identification of missing values and the calculation of null percentages for each column. Columns with a high proportion of missing data or low analytical relevance were excluded to avoid distorting the analysis.

For columns with a low percentage of missing values, a context-aware imputation strategy was applied. Average values were calculated based on:
- Property type  
- Furniture status  
- Average usable area  

These averages were then used to estimate prices and replace missing values, preserving data integrity while maintaining representativeness.

Additional transformations were performed in Power BI using Power Query, including:
- Data type corrections  
- Standardization of categorical values  
- Creation of new conditional columns to improve segmentation  

Geographical logic was used to derive regional classifications from existing location fields, enabling regional-level analysis.

To further enhance the analytical value of the project, population density data was sourced from external public datasets and integrated into the model. This enrichment allows direct comparison between population concentration and the volume of properties available for sale, adding a demographic dimension to the analysis.


## Key Market Insights

The dashboards reveal several relevant insights about the Portuguese real estate market:

- Lisbon and Porto account for approximately 40% of all properties currently listed for sale, highlighting a strong concentration of market supply in the two main metropolitan areas.
- The total market volume, calculated as the sum of all listed property prices, exceeds €50 billion, reflecting the scale and economic relevance of the active real estate market.
- There are currently around 135,000 properties listed for sale nationwide, providing a comprehensive snapshot of market supply.
- Lisbon, Faro, and the island of Porto Santo exhibit the highest apartment prices per square meter, indicating strong demand and pricing pressure in these regions.
- In the housing segment, Faro stands out as the most expensive region, with average prices close to €6,000 per square meter, likely driven by demand from foreign retirees, expatriates, and tourism-related investment.
- Castelo Branco, Guarda, and Viseu show the lowest land prices per square meter, typically ranging between €5 and €10, suggesting lower development pressure and more affordable entry points for land investment.
- Faro represents approximately 30% of all T0 (studio) listings, a pattern strongly associated with tourism demand and short-term rental (Airbnb) dynamics.
- In contrast, T1 apartments in Lisbon account for around 35% of published listings, potentially reflecting demand from university students and young professionals entering the labor market.


## Analytical Scope and Limitations
The analysis focuses exclusively on active listings, not on finalized transactions. As a result:
- Prices represent asking prices, not transaction values
- Market liquidity and negotiation effects are not captured

Nevertheless, the dataset provides a robust and timely representation of market supply and pricing signals.


## Conclusion
This project demonstrates how a structured and methodical data analysis approach can transform raw listing data into actionable insights. By combining rigorous data cleaning, contextual imputation, external enrichment, and interactive visualization, the analysis delivers a comprehensive view of the Portuguese real estate market from a supply-side perspective.

The resulting dashboards support informed decision-making for investors, analysts, developers, and real estate professionals, offering clarity on regional dynamics, pricing behavior, and market concentration.
