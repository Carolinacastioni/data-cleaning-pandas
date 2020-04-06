![Ironhack logo](https://i.imgur.com/1QgrNNw.png)

# Project | Data Cleaning and Manipulation with Pandas

## Introduction

In this project we will clean the messy file Shark Attack and will analyse the data in order to confirm or to deny our hypothesis. The project is compose by two jupyter files: `Clean.ipynb` and `Analysis.ipynb`. Below you can see the details about each file. 

## Hypothesis

The majority of surfers that are attacked by sharks in Australia are deadly injury. 

## Data Clean

- Import the CSV file Shark attack and create a dataFrame with the data.

- Start to explore the data: 
  Check the size of the file, the columns name and start to get an idea about the data we should deal with. 
   
- First Clean Action: Remove the duplicates
  Actually, we saw that we don't have duplicates on the database at this point.
  
- Second Action: Clean null values 
  Delete columns with null values and clean null rows. 
  
- Third Action: Clean some columns
  Check duplicated columns and delete those columns that we won't need for the analysis.
  
- Four Action: Changing teh Index
  Change the column "Case Number" to index.

- Fifth Action: Clean by string matching
  Aggrouping the following columns into key words: Type, Activity, Sex, Fatal, Age, Country, Species.
  
- Sixth Action: Categorization
  Create a called "Decada" that we can use on the analysis. We will build based on the column Year.
  
- Last Clean Actions:
      Remove the columns we now know we won't need for the analysis, Drop "not available" rows in the column Country, Remove "NaN" from the column Decada, check again if we have duplicates now that we have modified the data. 

- Export the clean database into a CSV file. First file had 25.723 X 24, clean file has 2.517 X 9.


## Data Analysis

- Import the CSV file cleaned on the `Clean.ipynb`.

- Insert the column Nº of cases: 
  This way we can sum up the number of shark attack cases. 
   
- Test the Group By function:
  In order to have a bigger picture of the Pivot table we are about to create.
  
- First Filter:  
  The activity column should be filter only by Surfing.
  
  Output:From 2.517 shark attacks, 1.051 were when people were Surfing. 
  
- Second Filter: 
  The country should be only Australia.
  
  Output: From the 1.051 shark attacks on Surfers, Australia has 197 cases of attack.
  
- Analysis: 
  From the 197 shark attackon surfers in Australia, only 24 were fatal, which proves that our hypothesis are wrong.
  

## Result

The majority of surfers attacked by a shark in Australia are not fatal.

