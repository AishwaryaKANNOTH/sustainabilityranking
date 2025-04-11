# sustainabilityranking


This project explores the follwing:
Which countries are actually doing well when it comes to sustainability?
Not just based on one metric like CO₂ emissions or renewable energy use — but based on a combination of economic, environmental, and social indicators. With guidance from global sustainability data, I set out to create a custom, data-driven Sustainability Score and explore global patterns.
I used a Kaggle dataset that compiles global sustainability indicators across dozens of countries and years. The dataset includes metrics such as:
Access to electricity
Renewable energy production and consumption
Life expectancy
National savings adjusted for environmental degradation
Annual CO₂ emissions

🛠️ Data Cleaning & Preprocessing
The dataset had
Dozens of columns with over 50% missing values
Country names repeated across multiple years
Some key metrics stored as strings instead of numbers

I dropped high-missing-value columns, filled other missing values with column means, and handled CO₂ emissions carefully since lower values indicate better sustainability. I also averaged metrics across multiple years to get a single score per country.

Creating a Custom Sustainability Score
I chose six core indicators to build a composite sustainability score:
Access to electricity (% of population)
Renewable electricity output (% of total electricity)
Renewable energy consumption (% of total energy)
Life expectancy at birth
Adjusted net savings (excluding pollution damage)
Reversed CO₂ emissions (lower = better)

Each of these was normalized using MinMax scaling, so values ranged between 0 and 1. I then averaged the scaled values to calculate a Sustainability Score for each country.

This project taught me that data science is part logic, part storytelling.

I learned:
How to clean real-world data and deal with missing values
How to engineer meaningful features from multiple variables
How to visually communicate insights in a clear and engaging way
How to question assumptions and be careful with bias in global comparisons
