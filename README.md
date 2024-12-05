# Ski Resort Capstone


Big Mountain Resort’s current business strategy is pricing tickets at a premium above the average market price and needs a data driven way to select price on tickets to increase revenue and profit. Big Mountain wants to capitalize on its facilities and does not currently know which are value-driving. (11 lifts, 2 T-bars, and 1 magic carpet for novice skiers). The Resort is also considering activities to reduce costs without undermining ticket price or support higher ticket price. There is $1.54 million in added operating costs this season due to an additional chair lift so that will affect profit margins unless we increase revenue by $1.54 million.



Big Mountain Ticket Pricing Strategy Proposal
By the end of this ski season, we aim to implement a data-driven pricing strategy tailored to Big Mountain’s market segment and competitive positioning based on other ski resorts in the US. This strategy seeks to boost revenue by at least $1.5 million by the end of the next ski season. Using a random forest model, we have determined the optimal Adult Weekend ticket price by analyzing Big Mountain’s facilities alongside the pricing and amenities of competitors.

In the "Notebooks" folder contain the data wrangling, eda, preprocessing and training and modeling complete with comments of our findings for each step of the process.


Key Insights and Recommendations
Optimal Ticket Price:
Our model suggests that the Adult Weekend ticket price should increase from the current $81.00 to $95.87, reflecting the high value of Big Mountain’s facilities. To cover the additional $1 million cost of a new chairlift, we propose a further increase of $0.88, resulting in a final ticket price of $96.75.

Model Performance:
The mean absolute error (MAE) of the random forest model is $10.39, indicating that price predictions are typically within $10.39 of the true value based on facilities.
The model demonstrates improved accuracy and consistency compared to a linear regression approach, which had a higher MAE of approximately $11.79.
Random forest modeling also revealed that fast quads, number of runs, snow-making acreage, and vertical drop are the most critical features influencing ticket price.

Current Pricing Misalignment:
Despite its competitive facilities, Big Mountain’s current ticket price of $81.00 significantly undercuts its modeled value. This discrepancy suggests a missed opportunity to align pricing with customer willingness to pay.

Facility Enhancements and Pricing Opportunities:
Adding a new run and increasing the vertical drop by 150 feet could justify a $1.99 price increase, even after accounting for the cost of the new chairlift.
Conversely, closing 10 ski runs would result in a $1.75 price decrease, highlighting the detrimental impact of reduced amenities on revenue potential.

Competitor Analysis:
Big Mountain excels in the key features identified as price drivers—fast quads, runs, snow-making area, and vertical drop—relative to competitors. However, its pricing strategy has not fully capitalized on this competitive advantage.
Model Selection and Validation


We developed and validated multiple models to ensure robust pricing recommendations:

Linear Regression:
Training/test MAE: $11.79
Cross-validation MAE: $10.50 (standard deviation: $1.62)
While effective, this approach showed greater variability and less accuracy compared to random forest modeling.

Random Forest:
Training/test MAE: $9.54
Cross-validation MAE: $9.64 (standard deviation: $1.36)
Preprocessing adjustments, such as median imputation for missing values and unscaled features, further optimized model performance.
Business Implications

Dynamic Pricing Opportunities:
The model provides a foundation for evaluating the revenue impact of various facility changes, enabling business analysts to simulate scenarios like run closures or expansions. For example:
Closing 3 runs has the same price impact as closing 4 or 5, while closing just 1 run has no effect.
Adding snow-making acreage or extending vertical drop height offers measurable price benefits.
Strategic Facility Investments:
Before implementing facility changes, we recommend evaluating associated costs, such as snow machine maintenance and construction expenses, to ensure profitability aligns with pricing strategy.


Conclusion
Big Mountain is underpricing its Adult Weekend tickets relative to its facilities and market position. By adopting the recommended price of $96.75 and considering facility improvements, the resort can both enhance its value proposition and achieve the target revenue increase of $1.5 million. Moving forward, the pricing model can serve as a decision-making tool to optimize the balance between facility investments and ticket pricing for sustained profitability.
