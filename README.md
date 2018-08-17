# convert-AIS-geopositions-to-CFD-cartesian

# Purpose: 
Convert all geopositions of different AIS ship tracks to cartesian coordinates to make transient (i.e. non-stationary) CFD simulations possible in which all ships move within the computational domain. If a vessel enters the CFD domain, it is repositioned at a distance of 2 minutes from the domain boundary. This allows the exhaust cloud in the chimney to develop long enough before the ship enters the CFD domain. This is possible because the entire domain must always be significantly larger than the area in which the actual analysis is performed (here referred to as computational domain) in compliance with CFD best practice guidelines.

Vessel tracks are read in from CSV files. 

# Challenge: 
The AIS tracks are partly longer than the CFD computational domain and each track enters or leaves the domain on different directions and times. Each vessel track characteristics needs to be considered. 
