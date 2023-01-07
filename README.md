# Practice_MLAgents_MovetoTarget
This project is to practice using mlagents to train a model in Unity.
> Folloeing this [youtube](https://www.youtube.com/watch?v=zPFU30tbyKs&t=691s) and [ML Agents](https://github.com/Unity-Technologies/ml-agents)

![picture 1](https://github.com/thirawat69/Practice_MLAgents_MovetoTarget/blob/main/README_PICTURE/normalPlatform.jpg?raw=true)

## Descriptions
The goal of this project is to get our agent (blue square) to collide with the target (yellow circle) using the mlagents tools kid.
The result after the training is good.

We have 4  objects:
1. Agent
2. Target
3. Platform
4. Wall

When the simulation starts, the Agent walks randomly in the X and Z directions. When the Agent walks collide the Target, it reward is +1 and the Platform turns red. When the Agent walks collide the Wall, it reward is -1 and the Platform turns red. Each Starting round Target is randomly respawned on the Platform.
- Before start training. Platform is gray.

![picture 1](https://github.com/thirawat69/Practice_MLAgents_MovetoTarget/blob/main/README_PICTURE/trainStart.jpg?raw=true)


- Starting train model. Agent is walk randomly and has a lot mistake.

![picture 2](https://github.com/thirawat69/Practice_MLAgents_MovetoTarget/blob/main/README_PICTURE/duringTrain1.jpg?raw=true)


- In the end. after training around 50,000 steps. Agent can walk efficiently.

![picture 3](https://github.com/thirawat69/Practice_MLAgents_MovetoTarget/blob/main/README_PICTURE/efficientWalk.jpg?raw=true)



## Getting Start
**Python environment**
```
py -3.7.9 -m venv venv
venv\Scripts\activate
python -m pip install --upgrade pip
pip install torch==1.7.0 -f https://download.pytorch.org/whl/torch_stable.html
pip install mlagents==0.29.0
mlagents-learn --help
```

**Unity envirament**
Editor version `2020.3.38f1`
Package `ML Agent v2.2.1-exp.1`

**Visual Studio Community **
Version `2019` `16.11.18`

**Train command**
```
mlagents-learn
```
```
mlagents-learn --force
```
```
mlagents-learn --run--id=Train05
```

<p align="right">(<a href="#top">back to top</a>)</p>

