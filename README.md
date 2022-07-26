# Awesome Neural Radiance Fields [NeRF] and Implicit Representations
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

A curated list of NeRF and Implicit Representations projects. This long-term repo is frequently updated and contains latest works (including tutorials, lectures, papers, codebases). Stay tuned!


## Contributing
If you have any suggestions, feel free to send [pull requests](https://github.com/salykovaa/awesome-nerf/pulls)! Modify the `README.md` and follow the format
``` 
[title](link_to_pdf) <br> authors <br> *conference year* | [Project page](link) | [Github](link) | Additional links ...
``` 

[Instant Neural Graphics Primitives with a Multiresolution Hash Encoding](https://arxiv.org/abs/2201.05989)
<br>
Thomas Müller, Alex Evans, Christoph Schied, Alexander Keller
<br>
*ACM Transactions on Graphics (SIGGRAPH) 2022* | [Project page](https://nvlabs.github.io/instant-ngp/) | [Github](https://github.com/NVlabs/instant-ngp)


## Table of contents
- [Survey](#survey)
- [NeRF Introduction](#nerf-introduction)
- [NeRF Papers](#nerf-papers)
  - [Improved training speed](#improved-training-speed)
  - [Improved rendering speed](#improved-rendering-speed)
  - [Unknown camera poses](#unknown-camera-poses)
  - [Object pose estimation](#object-pose-estimation)
  - [Unbounded, large-scale scenes](#unbounded-large-scale-scenes)
  - [Transparent objects](#transparent-objects)


## Survey
[Neural Fields in Visual Computing and Beyond](https://arxiv.org/abs/2111.11426) <br> Yiheng Xie, Towaki Takikawa, Shunsuke Saito, Or Litany, Shiqin Yan, Numair Khan, Federico Tombari, James Tompkin, Vincent Sitzmann, Srinath Sridhar <br> *Computer Graphics Forum (Eurographics 2022)* | [Project page](https://neuralfields.cs.brown.edu/) | [Recording](https://www.youtube.com/watch?v=hr2WQCs_P78)

[Lecture: Neural Scene Representation, Rendering, and Generation](https://www.youtube.com/watch?v=0KslwGsI9X8) <br> Gordon Wetzstein <br> *TUM AI Lecture Series, 2022*

[Advances in Neural Rendering](https://arxiv.org/abs/2111.05849) <br> Ayush Tewari, Justus Thies, Ben Mildenhall, Pratul Srinivasan, Edgar Tretschk, Yifan Wang, Christoph Lassner, Vincent Sitzmann, Ricardo Martin-Brualla, Stephen Lombardi, Tomas Simon, Christian Theobalt, Matthias Niessner, Jonathan T. Barron, Gordon Wetzstein, Michael Zollhoefer, Vladislav Golyanik <br> *SIGGRAPH 2021* | [Recording: part 1](https://www.youtube.com/watch?v=otly9jcZ0Jg) | [Recording: part 2](https://www.youtube.com/watch?v=aboFl5ozImM)

[Neural Volume Rendering: NeRF And Beyond](https://arxiv.org/abs/2101.05204) <br> Frank Dellaert, Lin Yen-Chen <br> *Arxiv 2021*

[Lecture: Implicit Neural Scene Representations](https://www.youtube.com/watch?v=__F9CCqbWQk) <br> Vincent Sitzmann <br> *TUM AI Lecture Series 2020*

[Seminar: Neural Rendering](https://www.youtube.com/watch?v=LCTYRqW-ne8) <br> *CVPR 2020* | [Morning session](https://www.youtube.com/watch?v=LCTYRqW-ne8) | [Afternoon session](https://www.youtube.com/watch?v=JlyGNvbGKB8)

[Seminar: Why Neural Rendering is Super Cool!](https://www.youtube.com/watch?v=-KGZmzP4P1I) <br> Matthias Niessner <br> *MIT CSAIL 2020*


## NeRF Introduction
[Lecture: Understanding and Extending Neural Radiance Fields](https://www.youtube.com/watch?v=nRyOzHpcr4Q) <br> Jon Barron <br> *TUM AI Lecture Series, 2020*

[NeRF: Neural Radiance Fields (10 min talk)](https://www.youtube.com/watch?v=LRAqeM8EjOo) <br> Ben Mildenhall, Pratul P. Srinivasan, Matthew Tancik, Jonathan T. Barron, Ravi Ramamoorthi, Ren Ng <br> *ECCV 2020*

[NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis (ML Research Paper Explained)](https://www.youtube.com/watch?v=CRlN-cYFxTk) <br> Yannic Kilcher <br> *2021*

[It’s NeRF From Nothing: Build A Complete NeRF with PyTorch](https://towardsdatascience.com/its-nerf-from-nothing-build-a-vanilla-nerf-with-pytorch-7846e4c45666) <br> Mason McGough <br> *Article from [towardsdatascience.com](https://towardsdatascience.com), 2021*

[Computer Graphics and Deep Learning with NeRF using TensorFlow and Keras](https://pyimagesearch.com/2021/11/10/computer-graphics-and-deep-learning-with-nerf-using-tensorflow-and-keras-part-1/) <br> Aritra Roy Gosthipaty and Ritwik Raha <br> *PyImageSearch 2021* | [Part 1](https://pyimagesearch.com/2021/11/10/computer-graphics-and-deep-learning-with-nerf-using-tensorflow-and-keras-part-1/) | [Part 2](https://pyimagesearch.com/2021/11/17/computer-graphics-and-deep-learning-with-nerf-using-tensorflow-and-keras-part-2/)


## NeRF Papers

[NeRF: Representing Scenes as Neural Radiance Fields for View Synthesis](https://arxiv.org/abs/2003.08934) <br> Ben Mildenhall, Pratul P. Srinivasan, Matthew Tancik, Jonathan T. Barron, Ravi Ramamoorthi, Ren Ng <br> *ECCV 2020* | [Project page](https://www.matthewtancik.com/nerf) | [Github](https://github.com/bmild/nerf) | [Video](https://www.youtube.com/watch?v=JuH79E8rdKc)

### Improved training speed

[Instant Neural Graphics Primitives with a Multiresolution Hash Encoding](https://arxiv.org/abs/2201.05989) <br> Thomas Müller, Alex Evans, Christoph Schied, Alexander Keller <br> *ACM Transactions on Graphics (SIGGRAPH) 2022* | [Project page](https://nvlabs.github.io/instant-ngp/) | [Github](https://github.com/NVlabs/instant-ngp)

[TensoRF: Tensorial Radiance Fields](https://arxiv.org/abs/2203.09517) <br> Anpei Chen, Zexiang Xu, Andreas Geiger, Jingyi Yu, Hao Su <br> *ECCV 2022* | [Project page](https://apchenstu.github.io/TensoRF/) | [Github](https://github.com/apchenstu/TensoRF) | [Video](https://www.youtube.com/watch?v=ujOMgaKV3lA)

[Point-NeRF: Point-based Neural Radiance Fields](https://arxiv.org/abs/2201.08845) <br> Qiangeng Xu, Zexiang Xu, Julien Philip, Sai Bi, Zhixin Shu, Kalyan Sunkavalli, Ulrich Neumann <br> *CVPR 2022* | [Project page](https://xharlie.github.io/projects/project_sites/pointnerf/index.html) | [Github](https://github.com/Xharlie/pointnerf) | [Video](https://www.youtube.com/watch?v=zmR9j-4AebA)

[EfficientNeRF: Efficient Neural Radiance Fields](https://arxiv.org/abs/2206.00878) <br> Tao Hu, Shu Liu, Yilun Chen, Tiancheng Shen, Jiaya Jia <br> *CVPR 2022* | [Github](https://github.com/dvlab-research/efficientnerf)

[PREF: Phasorial Embedding Fields for Compact Neural Representations](https://arxiv.org/abs/2205.13524) <br> Binbin Huang, Xinhao Yan, Anpei Chen, Shenghua Gao, Jingyi Yu <br> *Arxiv 2022* | [Github](https://github.com/hbb1/PREF)


### Improved rendering speed

[R2L: Distilling Neural Radiance Field to Neural Light Field for Efficient Novel View Synthesis](https://arxiv.org/abs/2203.17261) <br> Huan Wang, Jian Ren, Zeng Huang, Kyle Olszewski, Menglei Chai, Yun Fu, Sergey Tulyakov <br> *ECCV 2022* | [Project page](https://snap-research.github.io/R2L/) | [Github](https://github.com/snap-research/r2l)

[NeurMiPs: Neural Mixture of Planar Experts for View Synthesis](https://arxiv.org/abs/2204.13696) <br> Zhi-Hao Lin, Wei-Chiu Ma, Hao-Yu Hsu, Yu-Chiang Frank Wang, Shenlong Wang <br> *CVPR 2022* | [Project page](https://zhihao-lin.github.io/neurmips/) | [Github](https://github.com/zhihao-lin/neurmips) | [Video](https://www.youtube.com/watch?v=PV1dCTWL5Oo)

[DIVeR: Real-time and Accurate Neural Radiance Fields with Deterministic Integration for Volume Rendering](https://arxiv.org/abs/2111.10427) <br> Liwen Wu, Jae Yong Lee, Anand Bhattad, Yuxiong Wang, David Forsyth <br> *CVPR 2022* | [Github](https://github.com/lwwu2/diver) | [Video](https://www.youtube.com/watch?v=jt9sLxc46P8)

[SqueezeNeRF: Further factorized FastNeRF for memory-efficient inference](https://arxiv.org/abs/2204.02585) <br> Krishna Wadhwani, Tamaki Kojima <br> *Arxiv 2022*

[Instant Neural Graphics Primitives with a Multiresolution Hash Encoding](https://arxiv.org/abs/2201.05989) <br> Thomas Müller, Alex Evans, Christoph Schied, Alexander Keller <br> *ACM Transactions on Graphics (SIGGRAPH) 2022* | [Project page](https://nvlabs.github.io/instant-ngp/) | [Github](https://github.com/NVlabs/instant-ngp)

[Point-NeRF: Point-based Neural Radiance Fields](https://arxiv.org/abs/2201.08845) <br> Qiangeng Xu, Zexiang Xu, Julien Philip, Sai Bi, Zhixin Shu, Kalyan Sunkavalli, Ulrich Neumann <br> *CVPR 2022* | [Project page](https://xharlie.github.io/projects/project_sites/pointnerf/index.html) | [Github](https://github.com/Xharlie/pointnerf) | [Video](https://www.youtube.com/watch?v=zmR9j-4AebA)

[EfficientNeRF: Efficient Neural Radiance Fields](https://arxiv.org/abs/2206.00878) <br> Tao Hu, Shu Liu, Yilun Chen, Tiancheng Shen, Jiaya Jia <br> *CVPR 2022* | [Github](https://github.com/dvlab-research/efficientnerf)

[PlenOctrees for Real-time Rendering of Neural Radiance Fields](https://arxiv.org/abs/2103.14024) <br> Alex Yu, Ruilong Li, Matthew Tancik, Hao Li, Ren Ng, Angjoo Kanazawa <br> *ICCV 2021* | [Project page](https://alexyu.net/plenoctrees/) | [Github](https://github.com/sxyu/volrend) | [Video](https://www.youtube.com/watch?v=obrmH1T5mfI)

[AutoInt: Automatic Integration for Fast Neural Volume Rendering](https://arxiv.org/abs/2012.01714) <br> David B. Lindell, Julien N. P. Martel, Gordon Wetzstein <br> *CVPR 2021* | [Project page](http://www.computationalimaging.org/publications/automatic-integration/) | [Github](https://github.com/computational-imaging/automatic-integration) | [Video](https://www.youtube.com/watch?v=GYxFYbih0PU)

[FastNeRF: High-Fidelity Neural Rendering at 200FPS](https://arxiv.org/abs/2103.10380) <br> Stephan J. Garbin, Marek Kowalski, Matthew Johnson, Jamie Shotton, Julien Valentin <br> *Arxiv 2021* | [Project page](https://microsoft.github.io/FastNeRF/) | [Video](https://www.youtube.com/watch?v=JS5H-Usiphg)

[NeX: Real-time View Synthesis with Neural Basis Expansion](https://arxiv.org/abs/2103.05606) <br> Suttisak Wizadwongsa, Pakkapon Phongthawee, Jiraphon Yenphraphai, Supasorn Suwajanakorn <br> *CVPR 2021* | [Project page](https://nex-mpi.github.io/) | [Github](https://github.com/nex-mpi/nex-code/) | [Video](https://www.youtube.com/watch?v=HyfkF7Z-ddA)

[KiloNeRF: Speeding up Neural Radiance Fields with Thousands of Tiny MLPs](https://arxiv.org/abs/2103.13744) <br> Christian Reiser, Songyou Peng, Yiyi Liao, Andreas Geiger <br> *Arxiv, 2021* | [Project page](https://creiser.github.io/kilonerf/) | [Github](https://github.com/creiser/kilonerf) | [Video](https://www.youtube.com/watch?v=PNh0LvMpovU)

[Baking Neural Radiance Fields for Real-Time View Synthesis](https://arxiv.org/abs/2103.14645) <br> Peter Hedman, Pratul P. Srinivasan, Ben Mildenhall, Jonathan T. Barron, Paul Debevec <br> *ICCV 2021* | [Project page](https://phog.github.io/snerg/) | [Github](https://github.com/google-research/google-research/tree/master/snerg) | [Video](https://www.youtube.com/watch?v=5jKry8n5YO8)

[NeuSample: Neural Sample Field for Efficient View Synthesis](https://arxiv.org/abs/2111.15552) <br> Jiemin Fang, Lingxi Xie, Xinggang Wang, Xiaopeng Zhang, Wenyu Liu, Qi Tian <br> *Arxiv 2021*

[Neural Sparse Voxel Fields](https://arxiv.org/abs/2007.11571) <br> Lingjie Liu, Jiatao Gu, Kyaw Zaw Lin, Tat-Seng Chua, Christian Theobalt <br> *NeurIPS 2020* | [Project page](https://lingjie0206.github.io/papers/NSVF/) | [Github](https://github.com/facebookresearch/NSVF) | [Video](https://www.youtube.com/watch?v=RFqPwH7QFEI)


### Unknown camera poses

[GARF: Gaussian Activated Radiance Fields for High Fidelity Reconstruction and Pose Estimation](https://arxiv.org/abs/2204.05735) <br> Shin-Fang Chng, Sameera Ramasinghe, Jamie Sherrah, Simon Lucey <br> *Arxiv 2022* | [Project page](https://sfchng.github.io/garf/) | [Github](https://github.com/sfchng/Gaussian-Activated-Radiance-Fields)

[BARF: Bundle-Adjusting Neural Radiance Fields](https://arxiv.org/abs/2104.06405) <br> Chen-Hsuan Lin, Wei-Chiu Ma, Antonio Torralba, Simon Lucey <br> *ICCV 2021* | [Project page](https://chenhsuanlin.bitbucket.io/bundle-adjusting-NeRF/) | [Github](https://github.com/chenhsuanlin/bundle-adjusting-NeRF)

[Self-Calibrating Neural Radiance Fields](https://arxiv.org/abs/2108.13826) <br> Yoonwoo Jeong, Seokjun Ahn, Christopher Choy, Animashree Anandkumar, Minsu Cho, Jaesik Park <br> *ICCV 2021* | [Project page](https://postech-cvlab.github.io/SCNeRF/) | [Github](https://github.com/POSTECH-CVLab/SCNeRF) | [Video](https://www.youtube.com/watch?v=wsjx6geduvk)

[GNeRF: GAN-based Neural Radiance Field without Posed Camera](https://arxiv.org/abs/2103.15606) <br> Quan Meng, Anpei Chen, Haimin Luo, Minye Wu, Hao Su, Lan Xu, Xuming He, Jingyi Yu <br> *ICCV 2021* | [Github](https://github.com/quan-meng/gnerf)

[NeRF--: Neural Radiance Fields Without Known Camera Parameters](https://arxiv.org/abs/2102.07064) <br> Zirui Wang, Shangzhe Wu, Weidi Xie, Min Chen, Victor Adrian Prisacariu <br> *Arxiv 2021* | [Project page](https://nerfmm.active.vision/) | [Github](https://github.com/ActiveVisionLab/nerfmm)


### Object pose estimation

[GARF: Gaussian Activated Radiance Fields for High Fidelity Reconstruction and Pose Estimation](https://arxiv.org/abs/2204.05735) <br> Shin-Fang Chng, Sameera Ramasinghe, Jamie Sherrah, Simon Lucey <br> *Arxiv 2022* | [Project page](https://sfchng.github.io/garf/) | [Github](https://github.com/sfchng/Gaussian-Activated-Radiance-Fields)

[Nerfels: Renderable Neural Codes for Improved Camera Pose Estimation](https://arxiv.org/abs/2206.01916) <br> Gil Avraham, Julian Straub, Tianwei Shen, Tsun-Yi Yang, Hugo Germain, Chris Sweeney, Vasileios Balntas, David Novotny, Daniel DeTone, Richard Newcombe <br> *CVPR 2022*

[NeRF-Pose: A First-Reconstruct-Then-Regress Approach for Weakly-supervised 6D Object Pose Estimation]([link_to_pdf](https://arxiv.org/abs/2203.04802)) <br> Fu Li, Hao Yu, Ivan Shugurov, Benjamin Busam, Shaowu Yang, Slobodan Ilic <br> *Arxiv 2022*

[INeRF: Inverting Neural Radiance Fields for Pose Estimation](https://arxiv.org/abs/2012.05877) <br> Lin Yen-Chen, Pete Florence, Jonathan T. Barron, Alberto Rodriguez, Phillip Isola, Tsung-Yi Lin <br> *IROS 2021* | [Project page](https://yenchenlin.me/inerf/) | [Github](https://github.com/yenchenlin/iNeRF-public) | [Video](https://www.youtube.com/watch?v=eQuCZaQN0tI)


### Unbounded, large-scale scenes

[Mip-NeRF 360: Unbounded Anti-Aliased Neural Radiance Fields](https://arxiv.org/abs/2111.12077) <br> Jonathan T. Barron, Ben Mildenhall, Dor Verbin, Pratul P. Srinivasan, Peter Hedman <br> *CVPR 2022* | [Project page](https://jonbarron.info/mipnerf360/) | [Video](https://www.youtube.com/watch?v=zBSH-k9GbV4)

[Block-NeRF: Scalable Large Scene Neural View Synthesis](https://arxiv.org/abs/2202.05263) <br> Matthew Tancik, Vincent Casser, Xinchen Yan, Sabeek Pradhan, Ben Mildenhall, Pratul P. Srinivasan, Jonathan T. Barron, Henrik Kretzschmar <br> *CVPR 2022* | [Project page](https://waymo.com/research/block-nerf/) | [Video](https://www.youtube.com/watch?v=6lGMCAzBzOQ)

[NeRFusion: Fusing Radiance Fields for Large-Scale Scene Reconstruction](https://arxiv.org/abs/2203.11283) <br> Xiaoshuai Zhang, Sai Bi, Kalyan Sunkavalli, Hao Su, Zexiang Xu <br> *CVPR 2022* | [Video](https://www.youtube.com/watch?v=BfrYuDv179Y)

[CityNeRF: Building NeRF at City Scale](https://arxiv.org/abs/2112.05504) <br> Yuanbo Xiangli, Linning Xu, Xingang Pan, Nanxuan Zhao, Anyi Rao, Christian Theobalt, Bo Dai, Dahua Lin <br> *ECCV 2022* | [Project page](https://city-super.github.io/citynerf/) | [Github](https://github.com/city-super/BungeeNeRF)

[Mega-NeRF: Scalable Construction of Large-Scale NeRFs for Virtual Fly-Throughs](https://arxiv.org/abs/2112.10703) <br> Haithem Turki, Deva Ramanan, Mahadev Satyanarayanan <br> *CVPR 2022* | [Project page](https://meganerf.cmusatyalab.org/) | [Github](https://github.com/cmusatyalab/mega-nerf)

[Urban Radiance Fields](https://arxiv.org/abs/2111.14643) <br> Konstantinos Rematas, Andrew Liu, Pratul P. Srinivasan, Jonathan T. Barron, Andrea Tagliasacchi, Thomas Funkhouser, Vittorio Ferrari <br> *CVPR 2022* | [Project page](https://urban-radiance-fields.github.io/) | [Video](https://www.youtube.com/watch?v=B973fam8Bag)


### Transparent objects

[NeRFReN: Neural Radiance Fields with Reflections](https://arxiv.org/abs/2111.15234) <br> Yuan-Chen Guo, Di Kang, Linchao Bao, Yu He, Song-Hai Zhang <br> *Arxiv 2022* | [Project page](https://bennyguo.github.io/nerfren/) | [Video](https://www.youtube.com/watch?v=uZin1Ynk6SM)

[Dex-NeRF: Using a Neural Radiance Field to Grasp Transparent Objects](https://arxiv.org/abs/2110.14217) <br> Jeffrey Ichnowski, Yahav Avigal, Justin Kerr, Ken Goldberg <br> *CoRL 2021* | [Project page](https://sites.google.com/view/dex-nerf) | [Unofficial implementation](https://github.com/salykovaa/instant-DexNerf)
