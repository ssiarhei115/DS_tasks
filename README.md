### Data Science Test Assignment (code_1.ipynb)
Recently we launched an advertising campaign that is targeted according to our occasion definitions. An occasion consists of a specific geographic region and time, with the goal being to identify certain audiences  (Eating Dinner, Going to a Concert, etc.). Each occasion consists of several line items representing different targeting settings inside the occasion. We are conducting a post-campaign analysis in order to understand how well we performed. You are going to help us to resolve one of the issues.
Task

You are provided with access to two tables:.

1. `stepptest.ds_test.push_history` - contains our targeting plan , with a column for line item ID and a column for day of week (dow) and hour of day (hod). 
2. `stepptest.ds_test.google_adv` - contains the campaign performance data with a column for zip code, local date and hour of day, line item ID, and impressions 
Your goal is to perform analysis of how accurately impressions were served at the planned dow/hod for the following line items:  20573186371, 20557215517, 20573098306, 20553552908. 

For a given dow/hod, we can consider that impressions were served correctly (according to our plan) if at least 100 impressions were served at this dow/hod for the whole duration of the campaign.

The result should be presented as four pairs of pivot tables (two for each line_item):  
    • First pivot table for particular line item: with hod - in rows, dow - in columns and sum of impressions for the whole duration of the campaign for each dow/hod as values, with coloring proportional to the impression sum; 
    • Second pivot table -  same format as first but instead of values in the cells we want them colored according to the accuracy of the match: green - dow/hod planned to target and got impressions (at least 100), red - planned to target but didn’t get impressions (less than or equal to 100) or not planned to target but got impressions (at least 100).


## Libraries & tools used
* see the requirements 
