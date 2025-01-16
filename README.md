# RL Volleyball Game

## Overview
A reinforcement learning-based volleyball game developed using Unity, where an agent learns to play volleyball through trial and error. The game is designed to implement reinforcement learning algorithms to improve agent behavior in the context of volleyball.

## Setup and Installation
### Prerequisites
- `Unity Editor (2020.3 or higher recommended)`
- `Unity ML-Agents Toolkit` (required for training models)

### Installation
- Clone or download the repository:
```bash
git clone git@github.com:Shade9378/rl_volleyball_game.git
```
- Navigate and add the downloaded project onto Unity Hub
- To install ML-Agents Package, follow the instruction: https://github.com/Unity-Technologies/ml-agents/blob/release_18_docs/docs/Installation.md

## To run the game
- Open the project in Unity.
- Press the ▶️ Play to start the simulation.
- Use the arrow keys/WASD to control the agent manually.

### Controls
| Action | Key |
|---------|--------|
| Move Forward |	W / Up Arrow |
| Move Backward |	S / Down Arrow |
| Move Left | Left Arrow |
| Move Right | Right Arrow |
| Rotate Left	| A |
| Rotate Right	| D | 
| Jump |	Space |

## To train the agent:
- Modify the training configuration in Assets/Config/trainer_config.yaml to suit your needs.
- Activate the virtual environment containing your installation of `ml-agents`.
- Navigate to your working directory, and run in the terminal:
```bash
mlagents-learn config/Volleyball.yaml --run-id=VB_1 --time-scale=1
```
- Press ▶️ Play in Unity to begin the training
- To monitor training progress with TensorBoard, from your working directory, in another terminal window, run:
```bash
tensorboard --logdir=results
```

## Acknoledgement
This project was built with the help of the guide from Coder One's "An introduction to machine learning with Unity ML-Agents": https://www.gocoder.one/blog/introduction-to-unity-ml-agents/
