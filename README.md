# Adaptive-gradient-method-from-L_0-to-L-infnity
This package is designed for the paper titled "Proximal Regularization of Deep Residual Neural Networks Applied to High-dimensional Genomic Data". 

It is utilized to facilitate adaptive proximal gradient methods using ResNets with various regularizers for four real high-dimensional genomic datasets (mice data, pig data, wheat data, and loblolly pine data). The regularizers included in this research are: L_0, L_1/2, L_2/3, MCP, SCAD, L_1, L_4/3, L_3/2, L_2, L_3, L_4, L_infty. We used BO to do parameters selection, and use to parallel computing to improve the computing efficiency. 

We explored a range of ResNet architectures aimed for 1D genomic data, including ResNet-5, ResNet-10, ResNet-15, ResNet-18, ResNet-20, ResNet-25. Each model consists of basic block modules with convolutional layers, batch normalization, and a final fully connected linear output layer. To incorporate regularization, we implemented a custom optimizer, which extends the standard PyTorch class. This optimizer combines an adaptive gradient step, similar to the Adam optimizer, with a subsequent proximal mapping step. Our implementation uses a momentum-like update with $\beta_1 = 0.1$ and $\beta_2 = 0.999$. After the gradient update, the optimizer applies a proximal operator to each weight, defined by a specific regularization function.

We also investige the traditional linear models with PGD using the same regulariers from L_0 to L_inf. All the codes are in the folder named "PGD". Another classical LightGBM also used as a baseline in this research. 

**Because the pig data is bigger than other two datasets and limited space, it is not possible for us to put all the datasets together. Please read the readme.txt in the folder named "data" to find the link for the pig data used in this research. 

