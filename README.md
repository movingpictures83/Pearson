# Pearson
# Language: R
# Input: CSV (abundances)
# Output: CSV (correlations)
# Tested with: PluMA 1.1, R 4.0.0
# Dependency: Hmisc 4.4.0

PluMA plugin to compute Pearson correlations (Pearson, 1896).  The plugin
accepts as input a CSV file where rows represent samples and columns represent
community members, and entry (i, j) represents the abundance of community member
j in sample i (this file should be normalized).

The plugin produces output Pearson correlations between community members
as another CSV file with both rows and columns representing members and entry
(i, j) the correlation value between member i and member j.

If the output file ends in ".unthresholded.csv", correlations will not be p-value
thresholded.  Otherwise a p-value threshold of 0.01 will be applied.
