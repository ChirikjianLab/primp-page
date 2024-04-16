[Sipu Ruan <sup>1</sup>](https://ruansp.github.io){:target="_blank"}, [Weixiao Liu <sup>2</sup>](https://www.linkedin.com/in/weixiao-liu-549081148){:target="_blank"}, [Xiaoli Wang <sup>1</sup>](https://github.com/lily983){:target="_blank"}, [Xin Meng <sup>1</sup>](https://twitter.com/i/flow/login?redirect_after_login=%2Fxinnnmeng){:target="_blank"},  and [Gregory Chirikjian <sup>1</sup>](https://www.eng.nus.edu.sg/me/staff/chirikjian-gregory-s/){:target="_blank"}

<small><sup>1</sup> Department of Mechanical Engineering, National University of Singapore, Singapore</small>

<small><sup>2</sup> Department of Mechanical Engineering, Johns Hopkins University, Baltimore, MD, USA</small>

## Introduction
![Cover figure]({{site.baseurl}}/resources/cover_figure.png "Cover figure"){:style="float: left;margin-right: 7px;margin-top: 7px;" height="40%" width="40%"} This paper proposes a learning-from-demonstration method using probability densities on the workspaces of robot manipulators. The method, named "PRobabilistically-Informed Motion Primitives (PRIMP)", learns the probability distribution of the end effector trajectories in the 6D workspace that includes both positions and orientations. It is able to adapt to new situations such as novel via poses with uncertainty and a change of viewing frame. The method itself is robot-agnostic, in which the learned distribution can be transferred to another robot with the adaptation to its workspace density. The learned trajectory distribution is then used to guide an optimization-based motion planning algorithm to further help the robot avoid novel obstacles that are unseen during the demonstration process. The proposed methods are evaluated by several sets of benchmark experiments. PRIMP runs more than 5 times faster while generalizing trajectories more than twice as close to both the demonstrations and novel desired poses. It is then combined with our robot imagination method that learns object affordances, illustrating the applicability of PRIMP to learn tool use through physical experiments.

## Links
- Paper: [Arxiv](https://arxiv.org/abs/2305.15761){:target="_blank"}, [OpenReview](https://openreview.net/forum?id=cpT4zTZPAS){:target="_blank"}
- Poster: [PDF](/resources/poster-rss-workshop-l4tamp-rsp-final.pdf){:target="_blank"}
- Code is available:
  - Source code: [MATLAB](https://www.github.com/ChirikjianLab/primp-matlab/){:target="_blank"}, [Python](https://www.github.com/ChirikjianLab/primp-python/){:target="_blank"} ([API reference]({{site.baseurl}}/resources/python-api/index.html))
  - Documentation

## Presentations
- [July 10, 2023; Daegu, South Korea] Presented in RSS 2023 workshop on [Learning for Task and Motion Planning](https://zt-yang.github.io/rss23-l4tamp-workshop/){:target="_blank"}

## Supplementary Video
(Coming soon)

## Citation
(Coming soon)
