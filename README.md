# Election_Analysis

## Overview of Election Audit

A Colorado Board of Elections employee, Tom, requested help to complete an audit of a recent local election. Votes were collected in three different ways (mail-in ballots, punch cards, and direct recording electric) which were then counted and compiled for analysis. Tom requested assistance with calculating the total number of votes cast in the election, the list of all candidates and all counties, the total votes by county and by candidate, and then, based on percentage of total votes, determining which candidate won and which county had the highest voter turnout.

## Resources
- Data Source: [election_results.csv](resources/election_results.csv)
- Software: Python 3.6.1, Visual Studio Code, 1.38.1

## Election Audit Results
Using Python, I wrote a code to compile all the votes and sort them by (1) who each vote was cast for, and (2) where each vote originated from. This was determined using "for" loops, to run through each row, create a list of unique candidate and county names, and then using an accumulator to total up the counts for each candidate and each county.

Here's an example:

![Example of for loop](https://github.com/ehalprin/election_analysis/blob/main/resources/for%20loop%20example.png)

I then used variables set to 0 to identify the winning candidate and county with the largest turnout - as the code looped through the various totals of each candidate and county, the ones with the most votes were set as the winning candidate or county:

![Example of largest county](https://github.com/ehalprin/election_analysis/blob/main/resources/Largest%20county%20example.png)

Finally, I printed the results as well as writing them into a text file for easy reference:

![Example of print and write](https://github.com/ehalprin/election_analysis/blob/main/resources/print_and_write.png)

The analysis of the election shows that:
- There were 369,711 votes cast in the election.
- The county results were:
  - Jefferson County represented 10.5% of the votes (38,855 total votes)
  - Denver County represented 82.8% of the votes (306,055 total votes)
  - Arapahoe County represented 6.7% of the votes (24,801 total votes)
- The county with the largest turnout was:
  - Denver County, which represented 82.8% of the votes, and 306,055 total votes.
- The candidates were:
  - Charles Casper Stockham
  - Diana DeGette
  - Raymon Anthony Doane
- The candidate results were:
  - Charles Casper Stockham received 23.0% of the votes (85,213 total votes)
  - Diana DeGette received 73.8% of the votes (272,892 total votes)
  - Raymon Anthony Doane received 3.1% of the votes (11,606 total votes)
- The winner of the election was:
  - Diana DeGette, who received 73.8% of the vote, and 272,892 total votes.

### Election Audit Summary

This script could be used in the future for additional elections. Elections with more than one candidate would simply require duplicating the candidate code, and creating new variables for the additional position (i.e. comptroller_name, comptroller_options, etc.). An election that had ballot questions (i.e. whether to legalize a particular substance) could also use this script -- instead of voting for a candidate, that data could be tabulated by changing the variables from string variables to boolean variables ("true" to legalize, "false" to not legalize). Any additional levels of location, like in elections across state lines, could also be calculated by duplicating the county code to tabulate additional geographic data (i.e. state_name, state_options, etc.).
