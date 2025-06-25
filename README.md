# Q-Learning Tic-Tac-Toe AI

An AI agent that learns to play Tic-Tac-Toe using reinforcement learning. The agent starts with zero knowledge and becomes nearly unbeatable through Q-Learning!

## How It Works

The AI uses **Q-Learning** to build a strategy table through trial and error:
- Plays 10,000 training games against random opponents
- Stores quality values for each move in every board state
- Balances exploration (trying new moves) vs exploitation (using known good moves)
- Learns optimal strategies without any pre-programmed game knowledge

## Key Components

- **QLearningAgent**: Implements the Q-Learning algorithm with epsilon-greedy action selection
- **Q-Table**: Maps board states to action values using defaultdict
- **Reward System**: +1 for wins, +0.5 for draws, 0 for losses

## Technical Details

**Learning Parameters:**
- Epsilon (ε): 0.1 - 10% exploration rate
- Alpha (α): 0.5 - learning rate  
- Gamma (γ): 0.9 - discount factor for future rewards

**State Representation:** Board positions converted to string keys for Q-table lookup

## Setup & Run

```bash
pip install numpy
python tictactoe_qlearning.py
```

The agent trains automatically, then you can play against it. Board positions are numbered 0-8.

## What's Cool About This

- Demonstrates reinforcement learning in action
- Shows how AI can develop strategies from scratch
- Only ~150 lines of code for a complete learning system
- Agent becomes surprisingly good at blocking and creating winning opportunities

have fun :)
