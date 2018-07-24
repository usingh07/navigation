## Learning algorithm

To train the agent the code provided on the course was used. It implements the **Deep Q-Learning ** algorithm, that uses neural networks to approximate the Q value for **action - state pairs**.

### Network architecture

* A network with two hidden layers was used with RELU activation. Each layer comprised of 64 nodes.

## Hyper-parameters

Following hyperparameters were used to train the agent.
* BUFFER_SIZE = int(1e5)  
* BATCH_SIZE = 64         
* GAMMA = 0.99            
* TAU = 1e-3              
* LR = 5e-4               
* UPDATE_EVERY = 4        


## Reward plot
Following reward plot was obtained when the agent was trained.

![](rewards.png)

## Ideas to improve the performance of the agent
* Further experimentation will be done with the agent using the Prioritized Experience Replay technique. 
* Agent will also be trained by taking direct screen pixels as the input.

