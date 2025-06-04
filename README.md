# Task-5: Exploratory Data Analysis (EDA)
## Objective
This project performs exploratory data analysis (EDA) on a Kaggle-style Titanic leaderboard dataset. The goal is to derive insights from submission scores, ranks, and submission frequencies.

**Tolls Used:** Jupyter Notebook
## Dataset
The dataset contains public leaderboard information including:
Rank: Leaderboard position of the team
TeamId / TeamName
Score: Accuracy or evaluation metric
SubmissionCount: Number of submissions by each team
TeamMemberUserNames

## Tasks Performed
1. **Initial Data Analysis**
   - Loaded dataset using `pandas`
   - Explored structure with:
     - `.describe()`
     - `.info()`
     - `.value_counts()` for `SubmissionCount`

2. **Visualizations using Seaborn & Matplotlib**
   - `pairplot`: Relationships between Rank, Score, and SubmissionCount
   - `heatmap`: Correlation matrix of numeric features
   - `scatterplot`: Rank vs Score distribution
   - `boxplot`: Score distribution by submission frequency
   - `histogram`: Overall distribution of scores
   - `boxplot`: General score spread and outliers
     
## Key Observations

- **Rank and Score** are strongly negatively correlated (higher score → better rank).
- **SubmissionCount** has weak or no correlation with performance.
- Participants with few submissions can still score very high.
- Most scores are tightly packed in the upper range, with a few outliers.
- The leaderboard is highly competitive with minimal score differences at the top.

## Summary of Findings

- **Performance matters more than submission frequency**.
- **High-quality models** often require fewer submission attempts.
- **Leaderboard rankings** are driven directly by score, not activity level.
- **Visualizations confirm** close competition and limited variation in top scores.
