## METRO ARTS GRANTS
# 1988-89 to 2017-18
# NSS Class Project: Power BI

Data source:  https://data.nashville.gov/Art/Metro-Arts-Grant-History/emcy-s884

**Data cleaning done in Excel** 
During the initial step of transforming the data, I made the following changes to make the data easier to query:
1. Class instructor "melted" the data to put dates in each row (not just as column headers)
2. I did some additional cleaning in Excel:
    A. I split out the dates from the funding source name (i.e., changed "Metro 2017-2018" to be fy_start 2017, and another column fy_end 2018).
    B. Some org. names were really long (120+ characters). I added a temporary field to count the length, then edited the longest ones so their names are fewer than 70 characters.
3. From 1988-89 to 2005-06, funding agency was named "Metro Arts & ABC yyyy-yy" (Arts Builds Communities). In later years the funding agency name was simply "Metro yyyy-yy".  I did a Find/Replace to change all to be "Metro yyyy-yy"   


**Data cleaning done in Power BI:**
1. A new program THRIVE was started in 2014-15 contintued through 2017-18 (the final year of the dataset). I created two sub-total columns for Metro vs Thrive grants.


