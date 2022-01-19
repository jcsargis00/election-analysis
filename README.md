# Election Analysis
## Purpose
The purpose of this project is to provide additional voter information to the election commission on behalf of Seth and Tom.   This technical analysis will start by using the candidate voting program and voting cvs file and add new subroutines to extract and report additional information pertaining to county voting results. The election commission has also requested a written analysis of the Election Audit (README.md)
Specific data requested is:
* The voter turnout for each county
* The percentage of votes from each county out of the total county
* The county with the highest turnout
* Winning candidate, vote count, percentage to be reported at the end of the new report
#
## Election-Audit Results
### Overview of Methodology Used
New code was added to the PyPoll code used for technical analysis of candidate votes to analyze votes with respect to counties where voting took place.  The voting data file (election_results.cvs) was opened from the Resources directory.  The file contained county information in column 2, index 1.  Code was added for the county data to be extracted and counted, specifically a decision statement with a logical operator to count counties and create a county list.  After the routine looped throught the voter data file, the county list contained 3 counties: Jefferson, Denver and Arapahoe.  Next, a script was written to keep track of the number of votes in each county.  The county votes and percentage of votes were calculated with another script.  Finally, the county results were printed and can be seen in the image below.
### New Results - County Votes Included in Analysis
Election results were saved to a text file called _election_results.txt in the analysis directory.
A summary of the Election-Audit is below, showing the total number and percentage of votes for each candidate, plus a breakdown by county (including the winning county) and a summary of the winner's vote count and percentage. Diane DeGette was the winning candidate with 272,892 votes (73.8% of the vote).  Denver County had the largest voter turnout (306,055 votes).

* 369,711 votes were cast
* Jefferson County had 38,855 votes (10.5% of total votes), Denver County had 306,055 votes (6.7% of total votes), Arapahoe County had 24,801 votes (6.7% of total votes)
* Denver County had the largest number of votes
* Percentage of total votes and number of votes each candidate
    - Charles Casper Stockham: 23.0% (85,213)
    - Diana DeGette: 73.8% (272,892)
    - Raymon Anthony Doane: 3.1% (11,606)
* Diane DeGette was the winning candidate with 272,892 votes (73.8% of the vote). 
#
![Election Results](https://github.com/jcsargis00/election-analysis/blob/main/analysis/electionresultcmdline.PNG)
## Election-Audit Summary
The script used for this technical analysis could easily be expanded with minor modification to be used for any election.  The structure is general enough to allow the scope of the analysis to be expanded.  Examples of other elections the script could be modified and used for include: state wide elections with multiple counties, local election with multiple candidates, national elections with multiple states and counties within.  The script is only limited by the data collected in the election_results.cvs file.  
