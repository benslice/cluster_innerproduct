Cluster 3.0 (1.5) Inner Product patch
=====================================

This patch provides an additional
similarity metric to "Cluster 3.0"
Namely, the ability to cluster
via a raw inner product.
*Command Line Only*
I don't use the gui, and it 
would presumably need some
additional changes before it
can use the additional options.

Similarity is defined as the inner product
(with NaNs set to 0) and 
Distance is defined as Zero - Similarity

This patch is intended to be applied to 
version 1.5 of Cluster version 3.0 
(don't ask me!)

which you can obtain here:
http://bonsai.hgc.jp/~mdehoon/software/cluster/software.htm
