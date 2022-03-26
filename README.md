# Layout_Simulation
Exercise: optimizing a machine layout in a new production hall (greenfield construction) -> minimizing the total transport way.<br>
Size of the hall: 5x5 units of length (1 unit == 3 meters); place is completely free (no obstacles)<br>
1 fix raw parts warehouse, 1 fix finished parts warehouse, 5 machines to be placed (each with a size of 1x1 units).<br>
5 different products will be produced on these machines, each with a different processing order through the machines.<br>
Based on the production plan the number of products for the next period is given & the material flow matrix was calculated.<br>
# Program:
The simulation results will be written to an excel file; if it allready exits, the new simulation results will be appended.<br>
The simulation is programmed object oriented, a class for the machines and the two warehouses was created.<br>
For the layout another class was created, which is initialized with a random layout.<br>
The warehouses spawn at the same exact place, after that the 5 machines spawn random (they respawn if they are on a used place)<br>
Each machines has a unique color to be distinguishable.<br>
Every layout is shortly visualized.<br>
The distance between each relevant machine is calculated and written to a matrix.<br>
This matrix is then multiplied with the material flow matrix to gain to total transport distance for a machines in the next period.<br>
The sum is taken to gain the desired number (total transport way) for the current layout.<br>
The results (x & y coordinates for each machine; distance between the machines, total transport way in units and meters) is appended to the dataframe.<br>
After the desired number of simulations were executed, the best results out of all simulations (current & previous) is displayed.<br>
