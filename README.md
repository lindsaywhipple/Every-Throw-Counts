# Every Throw Counts: Reimagining Athletics as a Team Sport

## Live Project
[View Live Project Here (RPubs)](https://rpubs.com/LindsayWhipple/EveryThrowCounts)

## Overview
This project reimagines track and field athletics as a team sport where every throw is summed rather than only the best. Built as part of DataCamp projects, it goes beyond the original course strucutre to include foul rate analysis, updates early/late performance splits, and Monte Carlo simulation.

## Objective
- Engineer meaningful scouting metrics including foul rate, consistency, and late-stage performance.
- Build a transparent, adjustable weighted scoring framework for athlete selection.
- Simulate match outcomes to evaluate the tradeoff between reliability and raw performance. 

## Dataset
Source: DataCamp (course-provided dataset)
Contains results from American athletes in horizontal jumps and throws from real track and field meets, including up to six individual thro distances per athlete per meet. 

## Tools and Technologies
- R
- tidyverse (dplyr, ggplot2)
- R Markdown (published via RPubs)

## Methodology
- Cleaned and reshaped wide-format throw data to long format.
- Identified and corrected inconsistent athlete name entries across meets.
- Engineered foul rate, success rate, early./late diff, and consistency metrics per athlete.
- Normalized all metrics to a 0-1 scale and applied justified weights for team selection.
- Validated selection framework via 1,000-match Monte Carlo simulation.
- Compared conservative vs. aggressive weighting strategies.

## Key Insights
- Foul rate is the most underappreciated metric in a summed-distance format -- a foul is a direct zero, not just a wasted throw.
- A reliability-first team selection strategy produced a 24.6% win rate vs. 96.5% for a distance-first strategy, revealing how weight choices encode competitive strategy.
- Late-flight zeros are largely structural absences due to field cuts, not fouls - conflating the two distorts athlete evaluation.
 
## Visualizations
- Foul rate distribution across the athlete pool.
- Selected athletes vs. pool average and best across all metrics.
- Match simulation margin distributions for both strategies.
 
## How to Run
1. Clone the repo.
2. Place athletics.csv in your working directory.
3. Open and knit AthleteScouting.Rmd in RStudio.
 
## Future Improvements
- Extend the framework to jumps and other throwing events for full roster construction.
- Incorporate opponent scouting to optimize lineups against specific teams.
- Model foul position as well as foul frequency for more granular risk assessment.
- Add date data to explore seasonal fatigue effects. 


