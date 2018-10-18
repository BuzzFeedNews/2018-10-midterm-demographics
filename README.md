# The Demographics of Close Congressional Races

This repository contains data and analyses supporting the BuzzFeed News article, "[Black Voters Are Underrepresented In This Year’s Biggest House Races](https://www.buzzfeednews.com/article/johntemplon/black-voters-underrepresented-in-biggest-midterms)," published October 18, 2018.

## Data

The data for this analyses came from two sources:

- __The U.S. Census__. The [`data/census`](data/census) directory contains three files: `table04b.xls` from the Census's [Voting and Registration in the Election of November 2016](https://www.census.gov/data/tables/time-series/demo/voting-and-registration/p20-580.html) and two files (`CD.csv` and `State.csv`) from the [Citizen Voting Age Population by Race and Ethnicity](https://www.census.gov/programs-surveys/decennial-census/about/voting-rights/cvap.html) (CVAP) estimates. The CVAP estimates are based on the American Community Survey from 2012-2016.

- __FiveThirtyEight__. The analyses use *FiveThirtyEight's* [House](https://projects.fivethirtyeight.com/2018-midterm-election-forecast/house/) and [Senate](https://projects.fivethirtyeight.com/2018-midterm-election-forecast/senate/) forecasts for the 2018 midterm election. BuzzFeed News downloaded the data in these calculations on October 18, 2018 at approximately 4pm U.S. Eastern time, and saved them to the [`data/fivethirtyeight`](data/fivethirtyeight) directory. The code used to collect and restructure the data can be found in the [`notebooks/00-download-fivethirtyeight-data.ipynb`](notebooks/00-download-fivethirtyeight-data.ipynb).

## Analysis

The article relies on two different analyses, each combining *FiveThirtyEight*'s forecasts and the Census's demographic data. The first analysis compares demographic differences in close House and close Senate races versus the rest of the nation; [the code can be found here](notebooks/01-analyze-close-races.ipynb). The second analysis quantifies relative voting power vis-a-vis race/ethnicity, using the "Voter Power Index"; [the code can be found here](notebooks/02-analyze-senate-voter-power-index.ipynb).

## Licensing

All code in this repository is available under the [MIT License](https://opensource.org/licenses/MIT). The data in the `data/census` directory was created by the U.S. Census and is released into the public domain.

## Questions / Comments?

Please contact John Templon at john.templon@buzzfeed.com.

Looking for more from BuzzFeed News? [Click here for a list of our open-sourced projects, data, and code](https://github.com/BuzzFeedNews/everything)
