# Adaptive-gradient-method-from-L_0-to-L-infnity
This package is designed for the paper titled "Proximal Regularization of Deep Residual Neural Networks Applied to High-dimensional Genomic Data". 

It is utilized to facilitate adaptive proximal gradient methods using ResNets with various regularizers for four real high-dimensional genomic datasets (mice data, pig data, wheat data, and loblolly pine data). The regularizers included in this research are: L_0, L_1/2, L_2/3, MCP, SCAD, L_1, L_4/3, L_3/2, L_2, L_3, L_4, L_infty. We used BO to do parameters selection, and use to parallel computing to improve the computing efficiency. 

Because the pig data is bigger than other two datasets and limited space, it is not possible for us to put all the datasets together. Please read the readme.txt in the folder named "data" to find the link for the pig data used in this research. 

