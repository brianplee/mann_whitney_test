# mann_whitney_test
Mann Whitney U-Test 

This method takes in a .CSV file as an argument, and performs the ranking, U-scoring, and test statistic (Z-value) calculations for the Mann Whitney U-test. 

Mann Whitney test:
  - Create a sorted list with all values from both sample sets, with each value identified by sample set (0 or 1).  
  - Rank all sorted values from 1 to n. 
  - For values that occur more than once, average the ranks of all occurrences of that value, and assign the average to all occurrences. 
  - U-score: for each value, increment its U-score by 1 for every value NOT from the same set that has a greater rank.
  - Add up all the U-scores for each individual sample set.  Select the lower U-score to calculate the Z-value. 

Interpretation:
  The null hypothesis states that a randomly selected value from one population is equally likely to be < or > a randomly selected value    from a second population.  If the resulting Z-value is greater than the Z-value associated with the chosen alpha, reject the null hypothesis.   
