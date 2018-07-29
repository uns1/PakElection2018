# Pakistan Elections 2018


## Data Files:

- Data for Pakistan's 2018 Elections for the National Assembly. *(Provincial Assembly data coming soon)*  
- Compiled/Scraped on 7/29/18 from the Election Commission of Pakistan's website. 
- Data for 270/272 NA Seats. Missing seats due to postponed elections.

| File | Description |
|--------|-------------|
| Election_2018_NA_Results_Raw.csv | Contain's all information found on the individual constituency result for National Assembly seats. The candidate, party & number of votes is in a list of dictionaries. If you're just looking for that information, use Election_2018_NA_VotingOnly.csv  |
| Election_2018_NA_VotingOnly.csv |  Candidate names, party, and votes for each constituency. Essentially, this is the votingResults column of the raw file broken down. |
| Election_2018_NA_winnerResults.csv | The winning candidates, their parties and votes for NA seats. Provided for ease of use if you just want to look at the winners |
| Election_2018_NA_runnerupResults.csv | The runner ups, their parties and votes for NA seats. Provided for ease of use if you just want to look at those that came second |

***

### File Description & Metadata

#### 1. Election_2018_NA_Results_Raw.csv
Contain's all information found on the individual constituency result for National Assembly seats.
Example URL scraped: https://www.ecp.gov.pk/ConstResult.aspx?Const_Id=NA-1&type=NA&Election_ID=10070&Election=GENERAL%20ELECTION%2025%20JUL%202018


| Column | Description |
|--------|-------------|
| numberOfCandidates | Number of candidates in the constituency as per the results page |
| polledToRegRatio | Ratio of votes polled to votes registered |
| registeredVoters | Number of registered voters |
| rejectedVotes | Number of rejected votes | 
| seat | Constituency e.g. NA-1 |
| seatName | Constituency Name |
| seatStatus | Result Status e.g. Announced |
| validVotes | Number of valid votes |
| votesPolled | Total number of votes polled |
| votingResults | This is a list of dictionaries containing candidate info, party, and number of votes |
| femaleTurnout | Female turnout %age |
| maleTurnout | Male turnout %age |
| totalTurnout | Total turnout %age |

#### 2. Election_2018_NA_VotingOnly.csv
If you just want the candidate names, party, and votes for each constituency, use this file instead.
Essentially, this is the votingResults column of the file above broken down.

| Column | Description |
|--------|-------------|
| candidateName | Number of candidates in the constituency as per the results page |
| candidateParty | Ratio of votes polled to votes registered |
| candidateVote | Number of registered voters |
| seat | Constituency e.g. NA-1 |
| seatName | Constituency Name |


***

- Data scraped from the web isn't always perfect. If you find any discrepancies, please let me know @ uns5@rutgers.edu

***

## TODO
- Update with complete data when made available on the ECP website.
- Scrape PA data.
- Add Integrity Checks/Tests.
- Upload Exploratory Analysis.

