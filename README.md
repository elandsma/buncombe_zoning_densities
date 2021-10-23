# Evaluating the correlation between Buncombe county zoning district and various racial population densities
This is a Data Science project that I am working on to assist a Political Science student with her senior thesis. 
The hypothesis is that Buncombe county zoning districts have an impact upon racial densities, or vice versa.
This is not my thesis - I am providing technical data science assistance, under the guidance of Dr. Brian Drawert.

Given geojson data for both census blocks and zoning districts, created an overlay intersection of census block data and Buncombe county zoning district data, to create a 3rd layer of children polygons, each of which has a one-to-one relationship with a single parent census block polygon and a single zoning district polygon.

The initial geojson data had to be converted from degrees to a consistent equal-area-projection coordinate system. This enables the ability to compute consistent polygon areas in square meters. 
Then, evaluate area of child layer as proportion of parent layers.
Used this proportion to get continuous theoretical population numbers and, subsequently, densities, for various popultions inside each 3rd layer child block.

Compute and view correlation coeefficient of various racial densities for each polygon, as compared to total population density.
