# Console-Finances

## What problem was solved
The financial records for a hypothetical company was analysed using codes written in JavaScript. The financial records was provided in an array composed of arrays with two fields namely; Date and Profit/Losses.

The information that was estimated from the analysis include;
1. Total number of months in the dataset
2. Net amount of Profit/Losses over the entire period
3. Average of changes in Profit/Losses over the entire period
4. The greatest increase in profits over the entire period with date included
5. The greatest decrease in Losses over the entire period with date included


## How was the problem solved 
The problem was solved sequentially as listed above.

1. Total Months
![Total number of months in dataset](./assets/images/Months.JPG)
As seen in the code above, the length property was called on the array (finances) to obtain total months in the data set

2. Net Profit/Losses
![Net Profit/Losses](./assets/images/Net%20profit.JPG)
The netPL was initalised to zero and for loop was used to iterate through the profit/losses data within the array to form a loop that adds consecutive profit/losses values and updates their cummulative sum in the variable netPL

3. Average of changes 
dateAndChange is an empty array at the beginning of the loop. A for loop was used to iterate through the finances array to calculate changes in profit or Losses value - which is the algebraic difference between consecutive P/L values within the array (see Line 108). In Line 109, each calculated change is appended onto the dateAndChange array together with the date corresponding to the current month. 
![Average of changes](./assets/images/Average%20of%20changes.JPG)

Another for loop was created (Line 114-117) to search through the new dateAndChange array and sum up the Change values. The sum obtained is then divided by the total months to obtain the average of changes value required. 