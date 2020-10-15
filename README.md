# Augmented Memory for Correlation Filters in Real-Time UAV Tracking

Matlab implementation of our Augmented Memory Correlation Filters (AMCF) tracker.

# Abstract

The outstanding computational efficiency of discriminative correlation filter (DCF) fades away with various complicated improvements. Previous appearances are also gradually forgotten due to the exponential decay of historical views in traditional appearance updating scheme of DCF framework, reducing the model’s robustness. In this work, a novel tracker based on DCF framework is proposed to augment memory of previously appeared views while running at real-time speed. Several historical views and the current view are simultaneously introduced in training to allow the tracker to adapt to new appearances as well as memorize previous ones. A novel rapid compressed context learning is proposed to increase the discriminative ability of the filter efficiently. Substantial experiments on UAVDT and UAV123 datasets have validated that the proposed tracker performs competitively against other 26 top DCF and deep-based trackers with over 40fps on CPU.

# Publication

AMCF tracker is proposed in our paper accepted by IROS 2020. Detailed explanation of our method can be found in the paper:

Yiming Li, Changhong Fu, Fangqiang Ding, Ziyuan Huang, and Jia Pan.

Augmented Memory for Correlation Filters in Real-Time UAV Tracking.

You can find this paper at: https://arxiv.org/abs/1909.10989.

If you want to refer to this paper, please cite it as follows:

@article{Li2019Augment,

author = {Yiming Li and Changhong Fu and Fangqiang Ding and Ziyuan Huang and Jia Pan},

title = {Augmented Memory for Correlation Filters in Real-Time UAV Tracking},

year = {2019},

journal = {arXiv:1909.10989}

}


# Contact

Yiming Li

Email: yimingli9702@gmail.com

Changhong Fu

Email: [changhong.fu@tongji.edu.cn](mailto:changhong.fu@tongji.edu.cn)

# Demonstration running instructions

This code is compatible with UAV123 benchmark and UAVDT benchmark. Therefore, if you want to run it in benchmark, just put AMCF folder in trackers, and config sequences and trackers according to instructions from UAV123 and UAVDT. 

# Results on UAV datasets

### UAV123@30fps

![](\results_OPE\UAV123\error_OPE.png)

![](\results_OPE\UAV123\overlap_OPE.png)

### UAVDT

![](\results_OPE\UAVDT\error_OPE.png)

![](\results_OPE\UAVDT\overlap_OPE.png)

# Acknowledgements

We thank the contribution of  Bertinetto, Ning Wang and  Lukezic for their previous work Staple, MCCT and CSR-DCF.  The feature extraction modules and some of the parameter are borrowed from the MCCT tracker (https://github.com/594422814/MCCT) and Staple tracker (https://github.com/bertinetto/staple) . The channel weight modules is borrowed from the CSR-DCF tracker. (https://github.com/alanlukezic/csr-dcf).
