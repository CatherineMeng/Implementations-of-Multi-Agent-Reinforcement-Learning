# Implementations-of-Multi-Agent-Reinforcement-Learning
Summary of MARL research paper with open-source implementations for characterizing MARL training time breakdown, speed, etc.

### Notes:
- Decentralized Learning assumess that each agent does not have full access to all the state and reward info of other agents. Agents usually do not share policy parameters (antonym: Centralized Training (+ Decentralized Execution, CTDE)).
- Pre-defined Communication assumes that "who can talk to whom" is pre-determined and not to be dynamically learnt/changed during training (antonym: Learnable Communication).
- Partial-Structured Communication (antonym: All-to-all Communication)

## CTDE, Pre-defined Partial-Structured Communication
1. Graph convolutional reinforcement learning. 2020. [Paper📃](https://arxiv.org/abs/1810.09202),  [Code⌨️-DGN](https://github.com/PKU-RL/DGN)
    - Agents share the same policy network (GNN). 
    
## CTDE, Pre-defined All-to-all Communication
1. Learning multiagent communication with backpropagation. 2016. [Paper📃](https://arxiv.org/abs/1605.07736),  [Code⌨️-CommNet](https://github.com/KornbergFresnel/CommNet)
    - Agents share the same policy parameters, and are trained synchronously
2. Learning to Communicate with Deep Multi-Agent Reinforcement Learning. 2016. [Paper📃](https://arxiv.org/abs/1605.06676),  [Code⌨️-DIAL/RIAL](https://github.com/minqi/learning-to-communicate-pytorch)


## Decentralized Learning, Pre-defined Partial-Structured Communication
1. Deep multi-agent reinforcement learning with relevance graphs. 2018. [Paper📃](https://arxiv.org/abs/1811.12557),  [Code⌨️-MAGNet](https://github.com/tegg89/magnet)
    - Combines RL with GNN. 
    - Messages are weighted.
2. Learning transferable cooperative behavior in multi-agent teams. 2020. [Paper📃](https://arxiv.org/pdf/1906.01202.pdf),  [Code⌨️-Agent-Entity-Graph](https://github.com/sumitsk/marl_transfer)
    - Models simulation environemnts as agent-enttity graphs. Uses GNN. 

## Decentralized Learning, Pre-defined All-to-all Communication
1. Multi-agent reinforcement learning for networked system control. 2020. [Paper📃](https://arxiv.org/pdf/2004.01339.pdf),  [Code⌨️-NeurComm](https://github.com/cts198859/deeprl_network)

