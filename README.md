# t-SNE-for-images

t-SNE is a popular method for exploring high-dimensional data, 
introduced by van der Maaten and Hinton in 2008 [1]. The technique has an almost magical ability to create compelling
two-dimensonal “maps” from data with hundreds or even thousands
of dimensions.


The goal is to take a set of points in a high-dimensional space and find a faithful representation
of those points in a lower-dimensional space, typically the 2D plane. 
The algorithm is non-linear and adapts to the underlying data, performing different transformations
on different regions. Those differences can be a major source of confusion.

A second feature of t-SNE is a tuneable parameter, “perplexity,” which says (loosely) how to balance 
attention between local and global aspects of your data. The parameter is, in a sense, a guess about 
the number of close neighbors each point has. The perplexity value has a complex effect on the resulting 
pictures. The original paper says, “The performance of SNE is fairly robust to changes in the perplexity,
and typical values are between 5 and 50.” But the story is more nuanced than that. Getting the most from t-SNE 
may mean analyzing multiple plots with different perplexities.

## This repo:
This repository utilizes t-SNE to reduce the dimensionality of an image to 2D,
and visualise the clustering of images with the reduced dimensionality.
The image dataset used here is the UCI ML handwritten digits dataset available in sklearn.datasets as load_digits.


### ref: https://distill.pub/2016/misread-tsne/
