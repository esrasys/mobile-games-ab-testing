# Mobile Games A/B Testing

A product experimentation project analyzing how a progression design change affects player retention and activity in a mobile game.

## Project Goal

The goal of this project is to evaluate whether moving the first progression gate in the Cookie Cats mobile game from level 30 to level 40 improves player retention and player activity.

This analysis is framed as a product decision problem, combining behavioral analytics, statistical testing, and business-oriented interpretation.

## Business Context

In mobile games, progression barriers can influence both player frustration and long-term engagement. A design change that appears to reduce friction may improve early user experience, but it can also reduce challenge and weaken retention.

This project examines whether the treatment version (`gate_40`) performs better than the control version (`gate_30`) in terms of:

- day-1 retention
- day-7 retention
- player activity (`sum_gamerounds`)

## Dataset

This project uses the **Cookie Cats A/B Testing** dataset.

Main variables include:

- `userid`
- `version`
- `sum_gamerounds`
- `retention_1`
- `retention_7`

## Analytical Workflow

1. Data review and validation  
   - checked structure, summary statistics, missing values, and group balance

2. Exploratory analysis  
   - compared retention and player activity across control and treatment groups

3. Statistical testing  
   - used proportion-based hypothesis testing for retention metrics

4. Behavioral interpretation  
   - analyzed player activity distributions and interpreted findings in a product context

5. Recommendation  
   - translated the experiment results into a practical product decision

## Key Findings

- The difference in **day-1 retention** was not statistically significant.
- The difference in **day-7 retention** was statistically significant, with the control group (`gate_30`) performing better.
- Player activity was highly right-skewed in both groups, but the control group showed slightly stronger engagement overall.
- The results suggest that moving the first gate from level 30 to level 40 did not improve retention and may have weakened medium-term engagement.

## Final Recommendation

Based on the results, keeping the gate at **level 30** appears to be the better product decision.

The treatment version did not improve short-term retention and performed worse on day-7 retention, which is a more meaningful indicator of sustained engagement.

## Tools Used

- Python
- pandas
- numpy
- matplotlib
- seaborn
- statsmodels

## Repository Contents

- `mobile_games_ab_testing.ipynb` — full notebook with analysis and interpretation
- `README.md` — project overview and findings

## Project Positioning

This project demonstrates practical skills in:

- A/B testing
- product analytics
- behavioral analysis
- retention analysis
- statistical testing
- data storytelling
- decision-oriented insight generation
