# cluster-analysis-of-JHU-PHD-graduate-careers
Cluster analysis of JHU PHD programs based on careers 

This analysis used data from the [Coalition for Next Generation Life Science](http://nglscoalition.org/coalition-data/#close)

This analysis examines if PHD programs can be clustered together based on similarities in career sector (academia, industry, government, and non-profit) 10 years post-graduation. What programs share a similar career profile and what might be the cause of that? 

## Analysis Steps
1. Data was taken from original Excel file given in class (there was a technical issue in using the Tabula software).
2. Data was cleaned using the ctrl + e command to separate data into the correct columns.
3. Standard deviation and mean was calculated for each column.
4. Data was normalized using a z-score which was calculated for each percentage of graduates in each career sector.
5. Three clusters were randomly selected and their associated z-scores for each sector was pulled up using VLOOKUP.
6. SUMXMY2 function was called to find the sum of the differences between the z-score array of the choosen cluster node and the selected node.
7. All SUMXMY2 results were summed together.
8. The solver function was then used to change the three nodes in order to minimize the sum of differences of squares. 
9. The data was then sorted by cluster number to group each cluster together.

![alt text](https://github.com/yangnoah/analysis-of-baltimore-city-government-salary/blob/master/Graph.JPG)
