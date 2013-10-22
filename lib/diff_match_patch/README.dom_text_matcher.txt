I have modified the original diff-match-patch library, to return more data about the matches than the original version. 

This was needed for implementing searches for longer text segments, which are done by searching for multiple smaller segments, and aggregating the results. To aggregate the results, we need the individual lev. distances of the smaller matches, which the original version did not provide.

I have also added a workaround for a Chrome bug.
(Search for https://code.google.com/p/v8/issues/detail?id=2790 in the source.)
