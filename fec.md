# Markdown Assignment
## Semantha Norris

## Questions

1. Which industries contributed the most to the Republican and Democratic parties? How much was contributed to each party?
2. How much did donors from the Misc. Business sector contribute to the Democratic party? Which donors were based in Miami Lakes, FL?
3. What percentage of the tobacco industry’s donations does Philip Morris account for? How much is it?
4. Describe one potential story from this dataset that you’d find promising if this were a project you were working on. Give it a headline. Include up to three types of sources you would call to report out the story and a few of the questions you might ask.
5. What data might be suitable to join with this data to provide context or additional stories? Give me two examples.

## Answers

1. **Republican/Conservative contributed the most overall with $7,514,000. All of this money went to the Republican party, with $0 contributions to the Democratic Party.**
 <br> **The Media and Entertainment industry had the largest contribution to the Democrats, with $1,880,000**

Steps:
* Create a pivot table with the following settings for ROWS, COLUMNS, and VALUES
  *  ROWS = INDUSTRY
  *  COLUMNS = PARTY
  *  VALUES = AMOUNT "summarize by" "SUM"

!['Q1-Image1', 'Pivot table settings for question 1'](/Q1-Image1.png)

 *  Sort by "SUM of Amount in" "Grand total" to view the industry that contributed the most overall.

!['Q1-Image2', 'Sorting for Grand Total contributions'](/Q1-Image2.png)

*  Sort by "SUM of Amount in" "D" to then see the industry that contributed the most to the Democratics. 

!['Q1-Image3', 'Sorting for Democratic contributions'](/Q1-Image3.png)






