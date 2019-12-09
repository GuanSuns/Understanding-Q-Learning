# Understanding Reinforcement Learning


## The Overestimation Problem in Q-Learning
- **Source of overestimation**
    - Insufficiently flexible function approximation
    - Noise or Stochasticity (in rewards and/or environment)
- **Implementation**
    - Double Q-Learning
- **Papers**
    - Van Hasselt, Hado, Arthur Guez, and David Silver. "Deep reinforcement learning with double q-learning." Thirtieth AAAI conference on artificial intelligence. 2016.
    - Hasselt, Hado V. "Double Q-learning." Advances in Neural Information Processing Systems. 2010.


## The Sparse Reward / Reward Function Design Problem in RL
- **Papers**
    - Andrychowicz, Marcin, et al. "Hindsight experience replay." Advances in Neural Information Processing Systems. 2017.
    - Ding, Yiming, et al. "Goal-conditioned imitation learning." Advances in Neural Information Processing Systems. 2019.
    
    
## The Slow-Start Problem
- **Techniques**
    - Initialize parameters by imitation learning and proceed by Q-Filtering (allow outperform human expert)

- **Papers**
    - Hester, Todd, et al. "Deep q-learning from demonstrations." Thirty-Second AAAI Conference on Artificial Intelligence. 2018.


## Hard Exploartion Problem
