finding the relationship between $X,Y$ (two random variables) is a fundamental problem.
One way to express the dependency of these two is via the following:

$$
I(X;Y) := H(X) - H(X|Y) = H(Y) - H(Y|X)
$$
meaning the amount of entropy remained in X after knowing Y.

The main challenge we have here is that in practice we have a dataset of samples ${(x_i,y_i)}$ and we need to calculate MI from this dataset.

![[fig1-poole-2019.png

the above figure (from [[@pooleVariationalBoundsMutual2019]])



Two main categories of application for Mutual information

- Supervised Learning
$$ min_{\theta, EMP(X_i,\theta)<D} I(X,f_{\theta}(X))$$


- Unsupervised Learning 

$$ max_{\theta, constrians} I(X,f_{\theta}(X)),\; \text{By and large, }f_{\theta}(X)\; \text{is stocastic mapping}$$
Question is what is exactly the constrains for Unsupervised Learning?



