# Retail Sales Analytics

MSBA 738 Data Mining for Business Analytics  
Group W2: An Dang and Christian Cooper  
George Mason University, Fall 2026

## Project Overview

This project analyzes weekly retail sales patterns using sales outcomes, store characteristics, promotional markdown variables, holidays, and economic indicators. The goal is to connect historical sales drivers to practical managerial actions around inventory, staffing, promotion planning, and forecast adjustment.

## Business Questions

1. Which department, store, holiday, and economic factors help explain weekly sales?
2. Are markdown variables associated with higher weekly sales during the period when markdown data are available?
3. How do linear regression and decision tree models compare for prediction and interpretation?

## Repository Structure

```text
data/processed/
  GroupW2_Cleaned_FullPeriod.csv
  GroupW2_Cleaned_WithMarkdownPeriod.csv

presentation/
  W2_Presentation.pptx

rapidminer/
  Final_Decision_Tree.rmp
  Regression_with_markdown.rmp
  Regression_wo_markdown.rmp

report/
  MSBA738_GroupW2_Final_Report.docx
```

## Methods

- Joined Sales, Features, and Stores files into store-department-week records.
- Built full-period models without markdown variables.
- Built a markdown-period regression after filtering to the period when markdown fields became available.
- Compared linear regression and decision tree models using RMSE and MAE.

## Key Findings

- Department-level differences are a major driver of weekly sales.
- Store size is positively associated with weekly sales.
- The decision tree produced the lowest RMSE, while linear regression produced the lower MAE and clearer business interpretation.
- Markdown coefficients provide a sales signal, but they should not be treated as proof of profit impact without margin and promotion cost data.

## Data Source

The project is based on the Retail Data Analytics dataset from Kaggle:

https://www.kaggle.com/manjeetsingh/retaildataset

## Note

Large CSV and Office files are tracked with Git LFS.
