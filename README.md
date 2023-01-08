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
The netPL was initalised to zero and for loop was used to iterate through the profit/losses data within the array to form a loop that adds consecutive profit/losses values and updates them in the variable netPL