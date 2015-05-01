written by Soheil Bahrampour
March 2015

The Script is for task driven multimodal classification using l_{12} prior (joint sparsity).

It Performs dictionary learning (in first phase unsupervised, later supervised) on training data. Sparse codes generated are used as features which are feeded into multiclass quadratic
for classification. It should be straight forward to extend the code to cover other convex cost functions such as logistic regression. For more
information see the paper below:

Multimodal Task-Driven Dictionary Learning for Image Classification
Soheil Bahrampour, Nasser M. Nasrabadi, Asok Ray, W. Kenneth Jenkins
http://arxiv.org/abs/1502.01094

Please cite above paper if you use this code.

The joint sparse coding is solved using ADMM algorithm. The algorithm is implemented in c to gain speed advantage and is linked hear using a mex
file. Of course, one can use his own optimization algorithm instead of ADMM. The mex file is compiled for 64 system with a particulr articuture and it is not guarantted that it
can be used efficiently with other systeme.

Use the ClassificationMultiClassDecFusJoint.m file as the entry point.