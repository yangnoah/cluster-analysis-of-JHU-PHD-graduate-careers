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

![alt text](https://github.com/yangnoah/cluster-analysis-of-JHU-PHD-graduate-careers/blob/master/Program%20Cluster.JPG)

Cluster 1: PhD programs in the fields of biology and human anatomy (memorization heavy) 
Cluster 2: PhD programs with more of a quantitative focus such as engineering, statistics, and biomolecule interation (more problem-solving)
Cluster 3: Not really related to each other

This anaylsis shows that there are really two clusters of programs when differentiated by the career types 10 years afterwards. Since Cluster 2 has a more engineering and math focus, graduates in it would likely go to different sectors than those in Cluster 1 which has a more biology and anatomy focus.

For PhD students who are thinking about switching programs and wondering how it might affect their career in 10 years, this analysis shows them programs that would offer similar career trajectories. A person studying a program in Cluster 1 and like his/her career path should switch into a program in that cluster and not one in Cluster 2. 

This information can be used in practice to host career events/speaker sessions and have one session for each cluster since that cluster will be looking at similar career endpoints. 

For further analysis, data regarding career earnings, stress, growth, and relocation ease can be used to allow students to see what kind of programs offer similar quality of life. 
