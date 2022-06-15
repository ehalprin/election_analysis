# Election_Analysis

## Project Overview

A Colorado Board of Elections employee, Tom, requested help to complete an audit of a recent local election. Votes were collected in three different ways (mail-in ballots, punch cards, and direct recording electric) which were then counted and compiled for analysis. Tom requested assistance with the following tasks:

1. Calculating the total number of votes cast in the election.
2. Compile a list of all the candidates who received votes.
3. Calculate how many votes each candidate received.
4. Calculate the percentage of total votes that each candidate received.
5. Determine the winner of the election, based on popular vote.
6. Calculate how many votes were cast in each county.
7. Determine what county had the highest voter turnout.

## Resources
- Data Source: [election_results.csv](resources/election_results.csv)
- Software: Python 3.6.1, Visual Studio Code, 1.38.1

## Summary
Using Python, I wrote a code to compile all the votes and sort them by (1) who each vote was cast for, and (2) where each vote originated from. This was determined using "for" loops, to run through each row, create a list of unique candidate and county names, and then using an accumulator to total up the counts for each candidate and each county.

Here's an example:

![Example of for loop](https://github.com/ehalprin/election_analysis/blob/main/resources/for%20loop%20example.png)


The analysis of the election shows that:
- There were 369,711 votes cast in the election.
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
- The county results were:
      - Jefferson County represented 10.5% of the votes (38,855 total votes)
      - Denver County represented 82.8% of the votes (306,055 total votes)
      - Arapahoe County represented 6.7% of the votes (24,801 total votes)
- The county with the largest turnout was:
      - Denver County, which represented 82.8% of the votes, and 306,055 total votes.

## Challenge Overview

## Challenge Summary
