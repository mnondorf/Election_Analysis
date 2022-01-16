# Election_Analysis
## Overview of the Election Audit

The purpose of this project was to conduct an audit of the tabulated results for an election in a US Congressional Precinct in the state of Colorado in order to certify the results.

The requested outputs were:
* total number of votes cast
* total number of votes for each candidate
* pecentage of votes for each candidate
* winner of the election, based on the popular vote

## Election Audit Results

* A total of 369,711 votes were cast in this election.

* Jefferson County returned 38,855 votes, or 10.5% of the precinct vote total.
  Denver County returned 306,005 votes, or 82.8% of the precinct vote total.
  Arapahoe County returned 24,801 votes, or 6.7% of the precinct vote total. 

* Denver County had, by far, the largest number of votes.

* There were three candidates competing in this race. 
    Charles Casper Stockham received 85,213 votes (23.0%)
    Diana DeGette received 272,892 votes (73.8%)
    Raymon Anthony Doane received 11,606 votes (3.1%)

* Diana DeGette was the clear winner of this election, receiving over 73% (272,892) of all votes in her precinct.

![Results Image](Results.png)

## Election Audit Summary

The Python script used to conduct this analysis offers a clear and concise report of the candidates, reporting entities (in this case, counties), and vote counts. The percentage calculation that it returns makes identifying the winner and order of the runners up simple. With a few adjustments, it could easily be used to audit other elections. We recommend to the Colorado Election Commission that this Python script be used to certify any future elections it deems necessary to audit. 

#### Examples of how this script can be modified to be used for other elections

* import data files from other elections
* adjust the locations from which you pull the relevant candidate and vote information (i.e. candidate_name = row[2] in this example could be in row[1] in a different data set)
* include additional conditionals and outputs in the case of a potential candidate tie or a plurality contingency
* Adjust conditionals and outputs to show results for different voting areas, such as cities or neighborhoods