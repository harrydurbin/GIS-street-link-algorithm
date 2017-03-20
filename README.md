## GIS-street-link-algorithm
Created an algorithm to form street chain links on GIS data for a network of roads in Rio de Janeiro, Brazil. The algorithm assigns a numeric value to street chains that meet criteria of having a max distance separation between road line segments, and roads having a similar name (because GIS can have name typos). It was assumed that street link segments have a max allowable gap of 30 meters, and 97% name matching. 

To accomplish this, each line segment was assumed to be in a bounding box, and the corners of each line segment were linked together where possible based on the nearest distance. After each line segment was assigned to a numeric street link group, a shape file was created to view the results in GIS.

![alttag](https://github.com/harrydurbin/GIS-street-link-algorithm/blob/master/img/rio.png)
