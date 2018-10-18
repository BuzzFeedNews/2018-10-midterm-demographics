# The Demographics of Close Congressional Races

This repository contains the data and analysis for the BuzzFeed News article, "[Black Voters Are Underrepresented In This Year’s Biggest House Races](TKTKTK)," published October 18, 2018.

## Data

The data for this analysis came from two sources:

- __The U.S. Census__. The [`data/census`](data/census) contains three files: `table04b.xls` from the Census's [Voting and Registration in the Election of November 2016](https://www.census.gov/data/tables/time-series/demo/voting-and-registration/p20-580.html) and two files (`CD.csv` and `State.csv`) from the [Citizen Voting Age Population by Race and Ethnicity](https://www.census.gov/programs-surveys/decennial-census/about/voting-rights/cvap.html) (CVAP) estimates. The CVAP estimates are based on the American Community Survey from 2012-2016, so they have a little bit of a lag.

- __FiveThirtyEight__. The analysis uses *FiveThirtyEight's* [House](https://projects.fivethirtyeight.com/2018-midterm-election-forecast/house/) and [Senate](https://projects.fivethirtyeight.com/2018-midterm-election-forecast/senate/) forecasts for the 2018 midterm election. BuzzFeed News downloaded the data on October 18, 2018 at 11:30 am; you can find it in the [`data/fivethirtyeight`](data/fivethirtyeight) directory. The code used to collect the data can be found in these notebooks for [the Senate](notebooks/scrape-senate-voter-power-index.ipynb) and [the House](notebooks/scrape-house-race-details.ipynb).

## Analysis

The article relies on two different analyses done by combining the *FiveThirtyEight* and demographic data. The first analysis of the differences between close congressional races versus the rest of the nation [can be found here](notebooks/close-race-demographic-differences.ipynb). The second analysis quantifying relative voting power vis-a-vis race using the "Voter Power Index" [can be found here](notebooks/senate-voter-power-analysis.ipynb).

## Licensing

All code in this repository is available under the [MIT License](https://opensource.org/licenses/MIT). The data in the `data/census` directory is available under the [Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/) (CC BY 4.0) license. The data collected from *FiveThirtyEight* is licensed under their own terms.

## Questions / Comments?

Please contact John Templon at john.templon@buzzfeed.com.

Looking for more from BuzzFeed News? [Click here for a list of our open-sourced projects, data, and code](https://github.com/BuzzFeedNews/everything)