# Marketing A/B Testing
## Background
The data includes the results of an A/B test involving whether an ad was shown to a potential customer.
The majority of participants were exposed to the ad campaign (the experimental group) while the control group was exposed to either a PSA or blank space the same shape, size, and location that would otherwise be filled with the ad.

## Guiding Questions
- How much more will the company make from the ad campaign?
- Are the results significant enough to run the campaign?

## Comments on Testing
For a better experiment, we may want to change the probability of seeing an ad to be closer to even, or 50%.
This would lead to the least variance reduction, preventing dilution of the results.
A Sample Ratio Mismatch could invalidate the test at worst.
A Chi-Squared test should be used to determine if this has occurred.

## Data Dictionary
- Index: Row index
- User id: User ID (unique)
- Test group: If "ad" the person saw the advertisement, if "psa" they only saw the public service announcement
- Converted: If a person bought the product then True, else is False
- Total ads: Amount of ads seen by person
- Most ads day: Day that the person saw the biggest amount of ads
- Most ads hour: Hour of day that the person saw the biggest amount of ads

## Data Source
The dataset was acquired from the [Kaggle](https://www.kaggle.com/datasets/faviovaz/marketing-ab-testing?resource=download).

## Data License
[CC0: Public Domain](https://creativecommons.org/publicdomain/zero/1.0/)
