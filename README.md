# Marketing-AB-test

A statistical analysis of marketing campaign effectiveness using Python and A/B testing methodology.

## Project Overview
This project analyzes a marketing A/B test dataset to determine the effectiveness of different campaign types and identify patterns in user behavior that can inform marketing strategy.

## Dataset Details
- Index: Row index
- user id: User ID (unique)
- test group: If "ad" the person saw the advertisement, if "psa" they only saw the public service announcement
- converted: If a person bought the product then True, else is False
- total ads: Amount of ads seen by person
- most ads day: Day that the person saw the biggest amount of ads
- most ads hour: Hour of day that the person saw the biggest amount of ads
- Size: 588,101 users

## Data Quality
- No missing values in key variables
- No duplicate users confirmed
- Clean dataset ready for analysis

## Key Findings
### Statistical Results
- Significant association between campaign type and conversion (Chi-square test, p < 0.05)
- Highly significant difference in ad frequency between converters and non-converters (Mann-Whitney U test, p < 0.001)
- Non-normal data distribution confirmed through Shapiro-Wilk tests, validating the use of non-parametric methods

### Business Insights
- 96% of users saw traditional ads, 4% saw PSAs - uneven split limits comparative analysis
- Ad frequency directly correlates with conversion behavior
- Timing patterns identified in ad exposure across days and hours
- Clear optimization opportunities for frequency capping and budget allocation

### Technical Skills Demonstrated
- Statistical Testing: Chi-square, Mann-Whitney U, Shapiro-Wilk, Levene's tests
- Data Analysis: Python (pandas, numpy, scipy), exploratory data analysis
- Visualization: matplotlib, seaborn for clear data presentation
- A/B Testing: Proper experimental design evaluation and assumption checking
- Business Translation: Converting statistical findings into actionable insights
  

## Key Takeaways
1. Proper assumption checking is critical - data wasn't normally distributed, requiring non-parametric tests
2. Sample size matters - a large dataset (588K users) provided strong statistical power
3. Test design impacts insights - uneven 96/4 split, limited ability to compare campaign types
4. Statistical significance ≠ business significance - need to consider practical impact and cost implications
5. Frequency optimization presents a clear ROI opportunity - the relationship between ad exposure and conversion offers actionable insights
   
## Files
- marketing_AB_test.ipynb - Main analysis notebook
- marketing_AB.csv - Dataset
- README.md - This file

## Summary
The analysis successfully identified statistically significant patterns in user behavior that can inform marketing strategy. The methodology demonstrates proper A/B testing principles including assumption validation, appropriate test selection, and business-focused interpretation of results.
