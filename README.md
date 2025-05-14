# Map-Subpath-Locator
Given a trail and a query curve, find the best matching sub path of the trail


## Converting (WIP)
Handle regular OpenStreetMaps or other free mapping input, with one trail selected. This should be converted to an ordered set of points.

## Matching (WIP)
Given an ordered set of points T with fixed scaling and rotation, and a much smaller ordered set of points Q with fixed rotation but not scaling, find the subsets of T which Q has directed Hausdorff distance less than r too.

### Algorithm Outline
Filter most sections of T out. Note that for any starting point matching, all end point candidates lie in some band, so we can consider those points only.