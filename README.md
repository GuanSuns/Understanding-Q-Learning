# Understanding Reinforcement Learning


## The Overestimation Problem in Q-Learning
- **Source of overestimation**
    - Insufficiently flexible function approximation
    - Noise or Stochasticity (in rewards and/or environment)
- **Techniques**
    - [Double Q-Learning](https://github.com/GuanSuns/Understanding-Reinforcement-Learning/blob/master/The%20Overestimation%20Problem.ipynb)
- **Papers**
    - Van Hasselt, Hado, Arthur Guez, and David Silver. "Deep reinforcement learning with double q-learning." Thirtieth AAAI conference on artificial intelligence. 2016.
    - Hasselt, Hado V. "Double Q-learning." Advances in Neural Information Processing Systems. 2010.


## The Sparse Reward / Reward Function Design Problem in RL
- **Techniques**
	- HER
	- Goal-conditioned policy
- **Papers**
    - Andrychowicz, Marcin, et al. "Hindsight experience replay." Advances in Neural Information Processing Systems. 2017.
    - Ding, Yiming, et al. "Goal-conditioned imitation learning." Advances in Neural Information Processing Systems. 2019.
    
    
## The Slow-Start Problem
- **Techniques**
    - Initialize parameters with demonstrations or by imitation learning and proceed by Q-Filtering (allow outperform human expert)

- **Papers**
    - Hester, Todd, et al. "Deep q-learning from demonstrations." Thirty-Second AAAI Conference on Artificial Intelligence. 2018.


## Learn Expected Return vs Learn Value Distribution
- **Techniques**
    - Distributional Bellman and the C51 Algorithm
- **Benefit of Leanring Value Distribution**
	- Expected value might vastly overestimate due to some events with high rewards that happen less frequently. 
	- Though the expected future rewards of 2 actions are identical, their variances might be very different.
    - Leading to a much faster and more stable learning of the agent.
    - People can get more insights and knowledge of the agent by inspecting the learned distributions.
- **Papers**
    - Bellemare, Marc G., Will Dabney, and Rémi Munos. "A distributional perspective on reinforcement learning." arXiv preprint arXiv:1707.06887 (2017).
    - Blog: https://flyyufelix.github.io/2017/10/24/distributional-bellman.html


## Hard Exploartion Problem
