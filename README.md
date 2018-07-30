# Pakistan Elections 2018


## Data Files:

- Data for Pakistan's 2018 Elections for the National Assembly. *(Provincial Assembly data coming soon)*  
- Compiled/Scraped on 7/29/18 from the Election Commission of Pakistan's website. 
- Data for 270/272 NA Seats. Missing seats due to postponed elections.
- All data and analysis provided is provisional. The ECP website has a lot of missing/incorrect data. If you find any discrepancies, please let me know. 

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
| HDIRegion | The HDI region that corresponds to this seat. Please see the caveat about HDI data in the Scraper notebook. |
| HDIProvince | The province that the HDIRegion corresponds to |
| HDIValue2015 | The Human Development Index value (2015) for the HDIRegion |
| ImmunisationRate2015 | Percentage of fully immunized children between the age of 12 and 23 months based on record and recall. |
| SatisfactionWithHealth2015 | A household is regarded as deprived in ‘satisfaction with health facility’ if any of the household members did not use health care facility because it is costly, it does not suit, lacks tools or not enough facilities, or if any of the household member is not satisfied with the health facility. |
| ExpYearsOfSchooling2015 | Number of years of schooling that a child of school entrance age can expect to receive if prevailing patterns of age-specific enrolment rates persist throughout the child’s life. |
| MeanYearsOfSchooling2015 | Average number of years of education received by people ages 25 and older, calculated from education attainment levels using official durations of each level. | 
| LivingStd2015 | A composite index based on six household indicators related to access and quality of public services, household infrastructure and assets’ ownership. |
| HDIValue2013 | Human Development Index value in 2013 of the HDIRegion of the seat |
| HDIChangeInRank | Change in HDI ranking from 2013 to 2015 |
| firstName | Winner's name |
| firstParty | Party of the winner |
| firstVotes | Votes recieved by the winner |
| secondName | Runner up's name |
| secondParty | Runner up's party |
| secondVotes | Votes recieved by the runner up |
| thirdName | Name of the third placed candidate |
| thirdParty | Party of the third placed candidate |
| thirdVotes | Votes recieved by the third placed candidate |

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

