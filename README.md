# RealNVP
This contains simple 2D implementation of RealNVP.


The following diagrams are shown below. The first diagram is the inverse function mapping thats generated from our data. It should resemeble our Multivariate Normal Distribution, as shown on the figure to the right of it.

Below are samples being drawn from p(x) which was constructed by the chain of differentiable transformations of Z ~ N(0,I). Essentially it should model the original dataset. Normalizing Flows allow us to have exact maximum likelihood computation and data. That does not rely on latent space representation. 

This was modelled using a simple 2-D data, but can be extended to high dimensional data spaces like images and so on. 


Furthermore, As advised by the paper, we have alternated masking of the dimension through each coupling layer. The reason for doing this is that they want to ensuse that there is a chance of updates or change in the input dimension, where we use the same values as our input. The loss also seems to decrease. !



![REALNVP (1)](https://user-images.githubusercontent.com/17704242/226211172-c4765154-3646-4ad4-a7cc-7be1b715cfc8.png)
