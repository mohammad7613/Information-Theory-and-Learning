finding the relationship between $X,Y$ (two random variables) is a fundamental problem.
One way to express the dependency of these two is via the following:

$$
I(X;Y) := H(X) - H(X|Y) = H(Y) - H(Y|X)
$$
meaning the amount of entropy remained in X after knowing Y.

The main challenge we have here is that in practice we have a dataset of samples ${(x_i,y_i)}$ and we need to calculate MI from this dataset.

![[fig1-poole-2019.png]]