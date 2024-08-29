# buildings
a1_total_energy_initial
-uses IEA indicators to get intensity estimates for all economies out to 2100
-multiplies intensity by population projections to get total energy projection out to 2100
-plots comparison of total energy between IEA-derived, esto, and the 8th outlook
-generates csv file to be used in fuel split that has the total energy projected from IEA source to 2100

b1_fuel_split_ratio
-calculates the proportion of each fuel type in each subsector (srv and res) to the total fuel use

b2_fuel_split_projection
-uses fuel split proportion multiplied by total energy to get fuel amount estimates out to 2100
-compares fuel amounts between this estimate and the 1st iteration of the 9th outlook (8th results appended from 2022 onward to esto reported values)
-divided by the population for each fuel to get intensity, can use the intensity to project and make assumptions abou efficiency in the next part
  -adjustments in the next part could also be done to end use if we can figure out how to project that

c1_projection_adjust_function
-defines the function used to adjust (intensity) trajectory

c2_intensity_adjustments
-implements the f(x) for needed economies and fuels
-concatenates all files into one large file with intensity for each economy and fuel
-can multiply intensity by pop to get back to energy
