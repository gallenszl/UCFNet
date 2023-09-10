# UCFNet
This is the implementation of the paper Digging Into Uncertainty-based Pseudo-label for Robust Stereo Matching, `TPAMI 2023`, [\[Arxiv\]](https://arxiv.org/pdf/2307.16509.pdf).

See our conference implementation in this [\[website\]](https://github.com/gallenszl/CFNet)

The code will be available soon.

## Abstract
Due to the domain differences and unbalanced disparity distribution across multiple datasets, current stereo matching approaches are commonly limited to a specific dataset and generalize poorly to others. Such domain shift issue is usually addressed by substantial adaptation on costly target-domain ground-truth data, which cannot be easily obtained in practical settings. In this paper, we propose to dig into uncertainty estimation for robust stereo matching. Specifically, to balance the disparity distribution, we employ a pixel-level uncertainty estimation to adaptively adjust the next stage disparity searching space, in this way driving the network progressively prune out the space of unlikely correspondences. Then, to solve the limited ground truth data, an uncertainty-based pseudo-label is proposed to adapt the pre-trained model to the new domain, where pixel-level and area-level uncertainty estimation are proposed to filter out the high-uncertainty pixels of predicted disparity maps and generate sparse while reliable pseudo-labels to align the domain gap. Experimentally, our method shows strong cross-domain, adapt, and joint generalization and obtains **1st** place on the stereo task of Robust Vision Challenge 2020. Additionally, our uncertainty-based pseudo-labels can be extended to train monocular depth estimation networks in an unsupervised way and even **achieves comparable performance** with the supervised methods.


## Citation
If you find this code useful in your research, please cite:
```
@ARTICLE{ucfnet,
  author={Shen, Zhelun and Song, Xibin and Dai, Yuchao and Zhou, Dingfu and Rao, Zhibo and Zhang, Liangjun},
  journal={IEEE Transactions on Pattern Analysis and Machine Intelligence}, 
  title={Digging Into Uncertainty-Based Pseudo-Label for Robust Stereo Matching}, 
  year={2023},
  volume={},
  number={},
  pages={1-18},
  doi={10.1109/TPAMI.2023.3300976}}
```
```
@InProceedings{Shen_2021_CVPR,
    author    = {Shen, Zhelun and Dai, Yuchao and Rao, Zhibo},
    title     = {CFNet: Cascade and Fused Cost Volume for Robust Stereo Matching},
    booktitle = {Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)},
    month     = {June},
    year      = {2021},
    pages     = {13906-13915}
}
```
# Acknowledgements
Thanks to the excellent work GWCNet, Deeppruner, and HSMNet. Our work is inspired by these work and part of codes are migrated from [GWCNet](https://github.com/xy-guo/GwcNet), [DeepPruner](https://github.com/uber-research/DeepPruner/) and [HSMNet](https://github.com/gengshan-y/high-res-stereo).
