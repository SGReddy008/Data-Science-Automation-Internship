Employee Communication Sentiment Analysis

Project Overview

This project analyzes employee communication data to evaluate sentiment, identify top positive and negative communicators, and flag employees at potential flight risk.
Natural Language Processing (NLP), statistical scoring, and predictive modeling techniques were applied to extract meaningful insights.
The analysis helps HR teams monitor employee engagement, predict attrition risks, and make data-driven interventions.
________________________________________
🔑 Key Findings

Top 3 Positive Employees
1.	lydia.delgado@enron.com (Score: 184)
2.	john.arnold@enron.com (Score: 180)
3.	patti.thompson@enron.com (Score: 150)
   
Top 3 Negative Employees
1.	kayne.coulter@enron.com (Score: -103)
2.	rhonda.denton@enron.com (Score: -112)
3.	bobette.riner@ipgdirect.com (Score: -122)
   
Employees Flagged as Flight Risks

•	johnny.palmer@enron.com

•	don.baughman@enron.com

•	bobette.riner@ipgdirect.com

•	sally.beck@enron.com 

(Flagged for sending ≥4 negative messages within a 30-day rolling window)
________________________________________
📊 Insights from EDA

•	Most communications are neutral or positive, with negativity concentrated in a small subset of employees.

•	Message volume is unevenly distributed, with a few employees dominating interactions.

•	Monthly sentiment trends showed fluctuations, with noticeable spikes in negativity during certain months, possibly linked to organizational events.

•	Employees with persistent negativity overlap with those flagged as flight risks, strengthening confidence in the method.

________________________________________
⚙️ Methodology

Data Preprocessing

•	  Cleaned raw communication dataset.

•	  Converted dates, standardized text, and extracted monthly periods.
Sentiment Analysis

•	  Applied VADER sentiment analyzer.

•	  Classified each message as Positive, Neutral, or Negative.

Employee Scoring & Ranking

•	Assigned scores (+1 positive, 0 neutral, -1 negative).

•	Aggregated monthly and cumulative scores for each employee.

•	Ranked employees from most positive to most negative.

Flight Risk Identification

•	Flagged employees with ≥4 negative messages in 30 days as potential flight risks.
Predictive Modeling

•	Built a Linear Regression model to predict monthly sentiment scores.

•	Features: average message length, word count, monthly message volume, sentiment compound score.

•	Evaluated using MSE and R² score.

________________________________________
📌 Recommendations

1.	Early HR Interventions: Reach out to flagged employees with regular 1:1 check-ins and engagement programs.
  
3.	Continuous Monitoring: Build dashboards to track monthly sentiment and risk alerts.
  
5.	Model Improvements: Use advanced NLP (TF-IDF, BERT embeddings) and stronger ML models (Random Forest, Gradient Boosting).
   
7.	Holistic Analysis: Combine communication data with surveys, performance reviews, and HR data for well-rounded insights.
________________________________________
📂 Repository Structure

•	project_code.ipynb → Jupyter Notebook with full analysis.

•	Final Report.docx → Final detailed report.

•	README.md → This summary file.
________________________________________
🚀 Future Work

•	Implement transformer-based NLP for deeper semantic understanding.

•	Network analysis of communication patterns (who talks to whom).

•	Time-series forecasting for predicting shifts in employee sentiment.

________________________________________
👤 Author

•	Name: SANIKOMMU VENKATA GANESH REDDY

•	Contact: sgreddy008@gmail.com
