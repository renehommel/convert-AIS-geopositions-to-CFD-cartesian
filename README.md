# convert-AIS-geopositions-to-CFD-cartesian

# Purpose: 
Convert all geopositions of 6 different AIS ship tracks to cartesian coordinates to make transient (i.e. non-stationary) CFD simulations possible in which all ships move within the computational domain.

# Challenge: 
The AIS tracks are partly longer than the CFD computational domain and each track enters or leaves the domain on different directions and times. Each vessel track characteristics needs to be considered. 
