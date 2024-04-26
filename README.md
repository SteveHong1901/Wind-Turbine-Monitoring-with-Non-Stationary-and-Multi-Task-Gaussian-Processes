# Gaussian Processes for Wind Turbine Monitoring


Gaussian Processes are becoming a popular framework in monitoring wind tur- bines’ condition, especially for early fault detection, thanks to their expressiveness, robustness, and tractability. The performance of this type of model is significantly affected by the selection of kernel functions. Most of the existing research in wind turbine monitoring with Gaussian Processes employs standard stationary kernels, which are not optimal for wind power forecasting where patterns are inherently com- plex. This project aims to leverage scalable, non-stationary and multi-task kernel designs to apply Gaussian Process regression on a wind farm SCADA dataset and conduct a comparative analysis of their performance against baseline models.

Programming details and declarations
This project’s code is published under this link to Google Drive folder, which en- sures anonymity. The software and packages mentioned below have made significant contributions to the development of Chapter 6:
1. climate-kernel-learning by Lalchand et al. [2023]: This code base provides a fundamental framework for a hierarchical Gibb’s kernel. I expanded it into the full GSM kernel with two and three mixtures. The implementation include registering parameters, modifying the parameter constraints, rewrite the ker- nel composition to that of Remes et al. [2017] and update the inference and parameter whitening code.
2. GPyTorch by Gardner et al. [2018]: Deployed for learning and inference of RBF, SM and MTGP kernels. It is also used for VFE and FITC approximation, as well as for tensor manipulation and optimisation routines such as using ADAM.
3. Python Programming Language and commonly used packages including Matplotlib, NumPy, and Pandas.
