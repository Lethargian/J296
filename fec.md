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




