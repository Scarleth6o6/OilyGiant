# OilyGiant - Oil Extraction Investment Analysis

## Project Objective
OilyGiant plans to invest $100,000,000 USD in the development of 200 oil wells in one of three selected regions with high extraction potential. Each region has 500 identified points of interest, and the goal is to reduce this selection to a single region and the top 200 extraction points.

To achieve this, a machine learning model using linear regression will be trained to analyze the viability of each region by evaluating the expected gross profit. The reliability of the model will be validated using the bootstrapping technique, calculating the average profit per region and analyzing the 95% confidence interval. Additionally, risk assessments will be conducted to ensure that only regions with a loss risk below 2.5% are considered for investment.

## Conclusions

### **Profitability Analysis**
The analysis shows a significant difference in profitability between the regions. Region 1 has an average volume that is 26.83 units above the profitability threshold, whereas Regions 0 and 2 exceed it by 43.13 and 38.87 units, respectively. This suggests that Regions 0 and 2 have a significantly higher margin of profitability compared to Region 1.

### **Gross Profit Calculation**
To determine gross profit, the 200 highest-volume wells from each region were selected, their total reserves summed, and multiplied by $4,500 USD per thousand barrels of production. The investment cost of $100 million USD was then deducted to obtain the expected net profit for each region.

The results reveal a significant discrepancy among the three regions:
- **Region 0:** $38,821,157.44
- **Region 2:** $34,983,487.05
- **Region 1:** $24,824,861.69

Region 0 consistently demonstrates superior projected profitability compared to Regions 1 and 2. Although the difference between Regions 0 and 2 is not substantial, both are highly profitable relative to Region 1, which exhibits significantly lower returns. Given that Region 2 showed a higher average extraction volume during model validation, it remains a viable alternative; however, Region 0 is the preferred choice for investment.

### **Confidence Interval and Risk Assessment**
The 95% confidence intervals for each region further support the findings:
- **Region 0:** $38,116,930.62 to $39,509,833.19
- **Region 2:** $34,225,601.96 to $35,734,532.05
- **Region 1:** $24,790,020.52 to $24,858,825.78

These intervals indicate that the expected profits of Regions 0 and 2 have similar variability but consistently outperform Region 1. None of the three regions present a risk of negative returns, as the probability of loss is 0%. However, comparing average profit and confidence intervals, Regions 0 and 2 are the most profitable, with Region 0 being the top recommendation.

### **Model Accuracy and Recommendations**
The model's predictions align closely with actual data, as observed within the 95% confidence intervals. However, the root mean squared error (RMSE) indicates room for improvement in predictive accuracy. Alternative models or refinements could enhance precision.

Regarding the production threshold required to justify investment, Regions 0 and 2 stand out with differences of 43.13 and 38.87, respectively, while Region 1 shows a lower margin of 27.58. This further reinforces the viability of investing in Regions 0 and 2.

**Final Recommendation:** Given the analysis results, Region 0 is the most favorable choice for investment, as it consistently presents the highest average profit across all predictions. While Region 2 is a strong contender, the statistical support from confidence intervals favors Region 0. Therefore, the final recommendation is to proceed with investment in Region 0.


## 🛠 Technologies Used

- **Python**
- **Pandas, NumPy** (Data manipulation)
- **Scikit-learn** (Machine Learning models and evaluation)


## 🚀 How to Run the Project
### 1️⃣ Install Dependencies
```bash
pip install -r requirements.txt
```

### 2️⃣ Open the Jupyter Notebook
Run the following command to start Jupyter Notebook and open the project notebook:
```bash
jupyter notebook
```
Then, open the appropriate `.ipynb` file and execute the cells to train and analyze the models.

## 📁 Repository Structure
```
📂 SentimentAI
│-- 📂 data/                 # Dataset files
│-- 📂 models/               # Trained models
│-- 📂 notebooks/            # Jupyter notebooks for analysis and training
│-- requirements.txt         # List of dependencies
│-- README.md                # Project documentation
```


📂 **Repository:** [GitHub - SentimentAI](https://github.com/Scarleth6o6/proyecto_pozos_petroleros)
