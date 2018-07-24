### Project Details
_The README describes the the project environment details (i.e., the state and action spaces, how reward is decided, and when the environment is considered solved)._

For this project an agent have been trained in the task of colecting **yellow bananas** while evading **blue bananas**.

#### Action and State space
To collect the bananas the agent can perform the following actions (one at the time): **move forward**, **move backward**, **turn left** or **turn right**.

The state space consists on 37 vectors including the agent's velocity, along with ray-based perception of objects around the agent's forward direction.

#### Reward function
The agent gets a reward of **+1** for **yellow bananas** and **-1** for **blue bananas**.

The environment is considered solved when the agent receive an average reward (over 100 episodes) of at least **+13**.

### Learning Algorithm
_The report clearly describes the learning algorithm, along with the chosen hyperparameters. It also describes the model architectures for any neural networks._

To train the agent the code provided on the course was used. It implements the **Deep Q-Learning** algorithm, that uses neural networks to aproximate the Q value for **action - state pairs**.

### Getting Started
_The README has instructions for installing dependencies or downloading needed files._

1. Follow the [instructions](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md) to install Unity ML-Agents.

2. Navigate to the `p1_navigation/` folder, and run the command below to obtain a few more packages.
  ```
  pip3 install -r requirements.txt
  ```

3. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.

4. Place the file in the DRLND GitHub repository, in the `p1_navigation/` folder, and unzip (or decompress) the file.

## Instructions

_The README describes how to run the code in the repository, to train the agent. For additional resources on creating READMEs or using Markdown, see here and here._

1. Follow the instructions in `Navigation.ipynb` to get started with training your own agent!  To use a Jupyter notebook, run the following command from the `p1_navigation/` folder:

   ```
   jupyter notebook
   ```

   and open `Navigation.ipynb` from the list of files

2. On the notebook replace any appearance of **Banana unity Environment** (for instance `../Banana_Linux/Banana.x86_64`) with the path to your own Banana environment.

3. To start the training run the notebook code block under the **Train agent** header.

4. To test it run the code block under the **Test agent** header (you might need to restart the Kernel first)

