Website link: https://maryganey.github.io/LLMGeoBias/
# GPT and ZIP Code Demographic Bias Explorer

This project investigates how GPT-4.0 assigns ZIP codes based on user-level demographic information and whether these assignments reveal consistent patterns or biases related to race, gender, age, and rurality.  

## Project Overview

Using survey data and ACS ZIP-level demographics, GPT-4 was prompted to predict likely ZIP codes for users. This tool allows you to explore the results visually through interactive scatterplots and choropleth maps.  

**Key questions:**
- Are certain races or genders consistently placed into ZIP codes with higher or lower income?  
- Does GPT assign users to more rural or urban areas based on demographics?  
- Which demographic features most strongly shape GPT’s locational decisions?  

## Visualizations  
From the main HTML interface, you can:  
1. **Choose the plot type**: Scatterplot or Choropleth  
2. **Select a configuration**:  
   - `Full`: Includes all demographic features  
   - `No Race`, `No Gender`, etc.: Removes individual features from the input to observe their impact on GPT predictions  
All map outputs are color-coded based on prediction distance or demographic match to help interpret how features shift GPT’s reasoning.  

## Research Poster
You can view the full research summary and results in the academic poster below:  
[**Click here to view the research poster (PDF)**](POSTER_LINK_HERE)

## Demographic Summary
Our population was not evenly distributed:
- Age was skewed toward younger and middle-aged adults
- Gender was roughly balanced, with slight variation
- Race had unequal sample sizes, with White participants being overrepresented
This imbalance should be kept in mind when interpreting model outputs and bias patterns.

## Technologies Used

- **OpenAI GPT-4** for ZIP code prediction
- **Python (Pandas, Plotly, Seaborn)** for preprocessing and analysis
- **HTML + JavaScript** for interactive map selection
- **U.S. Census API** to enrich data with ZIP-level ACS context
---

Created by **Mary Ganey** – 2025 REU Program  
Supervised research on AI fairness and geographic bias
