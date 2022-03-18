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


Our idea about the application of the GAN pipline on balancing between usufull infomation and unusefull infomation based on our task in represntation learning:

One interesting application of Mutual information in GAN is to limit the information between the frist layer of discriminator and the last layer of discriminator. This technique conceptually limits the infomation by which the discriminator try to make the right decision about the distribution of input data. In this pipline, the generator doesn't have to recreate all the infomation in its output layer. It only needs to create the same peice of information of real data by which the disriminator come to right judjment about distribution.


In other view, we can say the discriminator map observations to other spaces in which only a certain peice of infomation related to the observation keeps intact and then try to make decision about all possible inputs creating the same disribution in the output space of the map. In this view, all the represenation of the real data containing the same pieces of infomation are treated in the same way by the discriminator and the generator only try to recreate one of these representation.


The above idea is induced from the title of 