[Sipu Ruan <sup>1</sup>](https://ruansp.github.io){:target="_blank"}, [Weixiao Liu <sup>2</sup>](https://www.linkedin.com/in/weixiao-liu-549081148){:target="_blank"}, [Xiaoli Wang <sup>1</sup>](https://github.com/lily983){:target="_blank"}, [Xin Meng <sup>1</sup>](https://twitter.com/i/flow/login?redirect_after_login=%2Fxinnnmeng){:target="_blank"},  and [Gregory Chirikjian <sup>1</sup><sup>,3</sup>](https://www.eng.nus.edu.sg/me/staff/chirikjian-gregory-s/){:target="_blank"}

<small><sup>1</sup> Department of Mechanical Engineering, National University of Singapore, Singapore</small>

<small><sup>2</sup> Department of Mechanical Engineering, Johns Hopkins University, Baltimore, MD, USA</small>

<small><sup>3</sup> Department of Mechanical Engineering, University of Delaware, Newark, DE, USA</small>

Published in __IEEE Transactions on Robotics (T-RO)__

## Introduction
![Cover figure]({{site.baseurl}}/resources/cover_figure.png "Cover figure"){:style="float: left;margin-right: 7px;margin-top: 7px;" height="40%" width="40%"} This paper proposes a learning-from-demonstration (LfD) method using probability densities on the workspaces of robot manipulators. The method, named PRobabilistically-Informed Motion Primitives (PRIMP), learns the probability distribution of the end effector trajectories in the 6D workspace that includes both positions and orientations. It is able to adapt to new situations such as novel via points with uncertainty and a change of viewing frame. The method itself is robot-agnostic, in that the learned distribution can be transferred to another robot with the adaptation to its workspace density. Workspace-STOMP, a new version of the existing STOMP motion planner, is also introduced, which can be used as a post-process to improve the performance of PRIMP and any other reachability-based LfD method. The combination of PRIMP and Workspace-STOMP can further help the robot avoid novel obstacles that are not present during the demonstration process. The proposed methods are evaluated with several sets of benchmark experiments. PRIMP runs more than 5 times faster than existing state-of-the-art methods while generalizing trajectories more than twice as close to both the demonstrations and novel desired poses. They are then combined with our lab's robot imagination method that learns object affordances, illustrating the applicability to learn tool use through physical experiments.

## Links
- **Paper**
  - [IEEE T-RO](https://ieeexplore.ieee.org/document/10502164){:target="_blank"}
  - [Arxiv](https://arxiv.org/abs/2305.15761){:target="_blank"}
  - [OpenReview (RSS 2023 workshop)](https://openreview.net/forum?id=cpT4zTZPAS){:target="_blank"}
  - [OpenReview (ICRA 2024 workshop)](https://openreview.net/forum?id=DTu0hqvWaU){:target="_blank"}
- **Poster**
  - [PDF](/resources/poster-rss-workshop-l4tamp-rsp-final.pdf){:target="_blank"}
- **Code**:
  - Source code: [MATLAB](https://www.github.com/ChirikjianLab/primp-matlab/){:target="_blank"}, [Python](https://www.github.com/ChirikjianLab/primp-python/){:target="_blank"}
  - Documentation: [Python API reference](/resources/python-api-v0.2.0/index.html){:target="_blank"}
- **Presentations** 
  - Presented in RSS 2023 workshop on [Learning for Task and Motion Planning](https://zt-yang.github.io/rss23-l4tamp-workshop/){:target="_blank"}

## Supplementary Video
<center>
  <iframe width="560" height="315" src="https://www.youtube-nocookie.com/embed/yp1CCNiqw7w?si=apYrSeUtubTUrf7y" title="YouTube video player" frameborder="0" allowfullscreen></iframe>
</center>

If the video cannot play, please visit [Media](https://ieeexplore.ieee.org/ielx7/8860/4359257/10502164/supp1-3390052.mp4?arnumber=10502164).

## Features of PRIMP:
### 1) Adaptation to new situations
- Novel **via-point** with uncertainty
<p align="center">
  <img src="https://github.com/ChirikjianLab/primp-page/assets/71541515/49382079-edd6-4c35-9731-4451c08c3799" alt="via point" width="400" />
</p>

- The equivariance property under the **change of viewing frame**
<p align="center">
<img src="https://github.com/ChirikjianLab/primp-page/assets/71541515/dca9589d-1cbc-487c-9779-e7037fe1449d" alt="view frame" width="400" />
</p>

- Avoid previously **unseen obstacles** while keeping the key features (The proposed Workspace-STOMP)
<p align="center">
<img src="https://github.com/lily983/primp-page/assets/71541515/501de672-9777-436c-a150-2746fdfabcd8" alt="avoid obs" width="400" />
</p>

### 2) Robot-agnostic
- Skills can be easily transferred to another robot by adapting to its workspace density
<p align="center">
<img src="https://github.com/lily983/primp-page/assets/71541515/f7e8b1fe-02b8-4d3d-9d51-0966a65c5f32" alt="robot agnostic" width="400" />
</p>

### 3) Combines with affordance learning
- Learning object affordance through physical interaction so that the skill can be applied to novel objects with the same affordance
<p align="center">
<img src="https://github.com/ChirikjianLab/primp-page/assets/71541515/b3fbd871-67f7-47a9-b260-ab1a33297b3f" alt="affordance" width="400" />
</p>

## Citation
```
S. Ruan, W. Liu, X. Wang, X. Meng and G. S. Chirikjian, "PRIMP: PRobabilistically-Informed Motion Primitives for Efficient Affordance Learning from Demonstration," in IEEE Transactions on Robotics, doi: 10.1109/TRO.2024.3390052.
```

BibTex
```
@ARTICLE{10502164,
  author={Ruan, Sipu and Liu, Weixiao and Wang, Xiaoli and Meng, Xin and Chirikjian, Gregory S.},
  journal={IEEE Transactions on Robotics}, 
  title={PRIMP: PRobabilistically-Informed Motion Primitives for Efficient Affordance Learning from Demonstration}, 
  year={2024},
  volume={},
  number={},
  pages={1-20},
  keywords={Trajectory;Robots;Probabilistic logic;Planning;Affordances;Task analysis;Manifolds;Learning from Demonstration;Probability and Statistical Methods;Motion and Path Planning;Service Robots},
  doi={10.1109/TRO.2024.3390052}}
```
