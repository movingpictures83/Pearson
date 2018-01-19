# Pearson
# Language: R
# Input: CSV (abundances)
# Output: CSV (correlations)

PluMA plugin to compute Pearson correlations (Pearson, 1896).  The plugin
accepts as input a CSV file where rows represent samples and columns represent
community members, and entry (i, j) represents the abundance of community member
j in sample i (this file should be normalized).

The plugin produces output Pearson correlations between community members
as another CSV file with both rows and columns representing members and entry
(i, j) the correlation value between member i and member j.
