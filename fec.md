# Markdown Assignment
## Semantha Norris

### Questions

1. Which industries contributed the most to the Republican and Democratic parties? How much was contributed to each party?
2. How much did donors from the Misc. Business sector contribute to the Democratic party? Which donors were based in Miami Lakes, FL?
3. What percentage of the tobacco industry’s donations does Philip Morris account for? How much is it?
4. Describe one potential story from this dataset that you’d find promising if this were a project you were working on. Give it a headline. Include up to three types of sources you would call to report out the story and a few of the questions you might ask.
5. What data might be suitable to join with this data to provide context or additional stories? Give me two examples.

## 1. Which industries contributed the most to the Republican and Democratic parties? How much was contributed to each party?

**_Republican/Conservative contributed the most overall with $7,514,000. All of this money went to the Republican party, with $0 contributions to the Democratic Party._**

**_The Media and Entertainment industry had the largest contribution to the Democrats, with $1,880,000._**

Steps:
1. Create a pivot table with the following settings for ROWS, COLUMNS, and VALUES
   *  ROWS = INDUSTRY
   *  COLUMNS = PARTY
   *  VALUES = AMOUNT "summarize by" "SUM"

!['Q1-Image1', 'Pivot table settings for question 1'](/Q1-Image1.png)

2. Sort by "SUM of Amount in" "Grand total" to view the industry that contributed the most overall.

!['Q1-Image2', 'Sorting for Grand Total contributions'](/Q1-Image2.png)

3. Sort by "SUM of Amount in" "D" to then see the industry that contributed the most to the Democratics. 

!['Q1-Image3', 'Sorting for Democratic contributions'](/Q1-Image3.png)


## 2. How much did donors from the Misc. Business sector contribute to the Democratic party? Which donors were based in Miami Lakes, FL?

**_Misc Business contributed $3,520,000 to the Democratic Party._**

**_Windmere Corp was based in Miami Lakes, FL._**

Steps:
1. Create a pivot table with the following settings for ROWS, COLUMNS, and VALUES
    *  ROWS = SECTOR
    *  COLUMNS = PARTY
    *  VALUES = AMOUNT "summarize by" "SUM"

!['Q2-img1', 'Pivot table settings for question 2'](/Q2-img1.png)

2. Find the row of "Misc Business" and the corresponding cell in column "D"

!['Q2-img2', 'Misc Business contributions to Democrats'](/Q2-img2.png)

3. In the Data Set create a filter in the "CITY" column to only see "Miami Lakes"

!['Q2-img3', 'Filter in city column to view Miami Lakes'](/Q2-img3.png)

!['Q2-img4', 'Results of filter in city column to view Miami Lakes'](/Q2-img4.png)


## 3. What percentage of the tobacco industry’s donations does Philip Morris account for? How much is it?

**_Philip Morris donations ($2,070,000) accounted for 68.54% of the tobacco industry's donations._**

Steps:
1. To get the _value_ that Philip Morris donated, create a pivot table with the following settings for ROWS, COLUMNS, and FILTER.
    *  ROWS = DONOR and "sort by" "SUM of Amount" 
    *  VALUES = AMOUNT "summarize by" "SUM"
    *  FILTER = INDUSTRY "filter by values" only choose "tobacco"

!['Q3-img1', 'Pivot table settings for question 3'](/Q3-img1.png)

!['Q3-img2', 'pivot table filter setting for question 3'](/Q3-img2.png)

!['Q3-img3', 'Results for question 3 value'](/Q3-img3.png)

2. To get the _percentage_ that Philip Morris' donations accounted for in the tobbacco industry donations:
    * Change VALUES to be "shown as" "%of grand total"

!['Q3-img4', 'Value setting for question 3 finding percentage'](/Q3-img4.png)

!['Q3-img5', 'Results for question 3 percentage'](/Q3-img5.png)


## 4. Clinton takes a stronghold on Unions and the Labor industry. 

The labor industry accounted for 15% of all contributions over $100,000 to the democratic party, while no contributions were made to the republican party. Clinton had the overwhelming support of labor unions in the East Coast, with all labor contributions coming from four states. Labor made up over half of the contributions Clinton's campaign received from DC.

#### Potential Sources
1. Communications Workers of America representative, to ask why they contributed to Democrats over Republicans, and what they think they will get from it. 
2. Actual workers. Do they agree with the contributions? Do they have preferences over candidates?
3. Workers from the South, or other areas that are Republican strongholds.
4. Expert that can speak to why labor favored democratic candidates. 
5. Policy analyst that can break down the campaign promises of the two candidates in relation to unions and labor. 

Steps:
1. Create a pivot table with the following settings for ROWS, COLUMNS, and VALUES
    *  ROWS = SECTOR
    *  COLUMNS = PARTY
    *  VALUES = AMOUNT "summarize by" "% of grand total"

!['Q4-img1', 'Pivot table settings for sector contributions'](/Q4-img1.png)

2. Create a pivot table with the following settings for ROWS, COLUMNS, and VALUES
    *  ROWS = STATE
    *  COLUMNS = PARTY
    *  VALUES = AMOUNT 
    *  FILTER = SECTOR (only check Labor)

!['Q4-img2', 'Pivot table settings for finding which states the Labor contributions came from'](/Q4-img2.png)

2. Create a pivot table with the following settings for ROWS, COLUMNS, and VALUES
    *  ROWS = STATE
    *  COLUMNS = SECTOR
    *  VALUES = AMOUNT (%of grand total)
    *  FILTER = PARTY (only check D)
    *  FILTER = STATE (only check DC)

!['Q4-img3', 'Pivot table settings for finding % of DC contributions to the Democrats Labor constituted'](/Q4-img3.png)

## 5. What data might be suitable to join with this data to provide context or additional stories?

1. Election results per state. This information could help to map and compare the regional effects of donations. Were there overlaps between the contributions and the results? 
2. Example 2 

