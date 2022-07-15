# Election_Analysis

## Project Overview

The Colorado election committee has requested additional information on top of the recent analysis completed for them in regards to the election audit. The board committee would now also like to determine the following:

1.The voter turnout for each county

2.The percentage of votes from each county out of the total count

3.The county with the highest turn out

The challenge is to use Python on the provided Election_results.csv file to calculate the desired statistics and print out the results to the terminal as well as in a text file that can be provided to the election committee.

### Background

The audit originally requested the following information:

1.The Total number of Votes cast

2.A Complete list of candidates who received votes

3.The total number of votes each candidate received

4.What is the percentage of votes each candidate won

5.Who is the winner of the election by the popular vote

After reviewing this information, the election committee has requested additional information with regards to the individual county showings. The challenge is to enhance the starter code used to develop the initial audit information to also include the additional requests.

Resources provided

Data Source: election_results.csv

Software: Python 3.7.6, Visual Studio code

## Election-Audit Results

1. BREAKDOWN OF VOTES BY COUNTY AND PERCENTAGE BY COUNTY

In order to calculate the breakdown of votes by county, a dictionary and list are created to keep county names as the key and accumulated votes by county as the value:

![image](https://user-images.githubusercontent.com/108489186/179317101-c5cd5e04-aadf-4395-a790-5c504bba5fd9.png)

Next while still in the for loop looking at all the records, when a new county name is encountered it is appended to the list

![image](https://user-images.githubusercontent.com/108489186/179317322-eb610402-e987-4f53-ad1e-9f82984ac3b3.png)

Finally a new variable to track votes by county is created and increased each time the county name shows up in the data file. The percentage of total votes for each county is now easy to calculate by dividing the total of the county by the overall total.

![image](https://user-images.githubusercontent.com/108489186/179317463-269bdf85-94a7-4cc4-99b6-af8f43fd7b69.png)

THE COUNTY WITH THE LARGEST VOTES

To identify the winning county, an if statement is used with a comparison variable within the for loop to check and see if the accumulated amount of votes in the dictionary is bigger than the prior winning county count and if so, replace the winning county count until the whole dataset has been processed. This comparison variable is initiated to 0 at the beginning of the code.

![image](https://user-images.githubusercontent.com/108489186/179317635-d978ce90-0850-487a-9121-4c411fbaaa23.png)

THE WINNING CANDIDATE

Given the prior calculations, it is a simple matter to determine the winner of the election. Similar logic to finding the county with the most votes is used to determine the candidate with the most votes as shown in the code below:

![image](https://user-images.githubusercontent.com/108489186/179317868-d473ffd3-7754-4b0a-8909-2243ee697c8a.png)

## ELECTION AUDIT SUMMARY

The script provided for this audit is able to calculate the total votes, votes by county and candidate and the percentage of total votes these account for. The script can be used on any file of undetermined length with similar data elements. With some modification, the script could also produce statistics of interest such as:

1.The votes by candidate by county - the election commission could then see which candidate won in each county and not just the overall winner

2.The script could also calculate the candidate winning the most counties which may be different than the overall popular vote

The code for this analysis can be found here:

![image](https://user-images.githubusercontent.com/108489186/179318388-69d991c4-f315-4b11-a520-3586abd9dacf.png)


A text file of the results of the analysis can be found here:

![Screenshot 2022-07-15 173801](https://user-images.githubusercontent.com/108489186/179318577-f1dfbfa4-bd93-4a7c-bce7-99e0b2a711e4.png)

















