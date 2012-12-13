Cluster 3.0 (1.5) Inner Product patch
=====================================

Benjamin VanderSluis
bvander@cs.umn.edu
December 13, 2012

This patch provides an additional
similarity metric to "Cluster 3.0"
Namely, the ability to cluster
via a raw inner product.


**Command Line Only**

I don't use the gui, and it 
would presumably need some
additional changes before it
can use the additional options.

Similarity is defined as the inner product
(with NaNs set to 0) and 
Distance is defined as 

Zero - Similarity/1000

Cluster needs the similarity to be less than one, 
so I've encoded the assumption that the inner product
will be less than 1000. This works for my applications,
but you may need to set that number to something
larger. See:

cluster.patch : lines 72-76

This patch is intended to be applied to 
version 1.5 of Cluster version 3.0 

which you can obtain here:
http://bonsai.hgc.jp/~mdehoon/software/cluster/software.htm
