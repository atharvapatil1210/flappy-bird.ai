# Flappy Bird AI Game

This project is a recreation of the classic Flappy Bird game using Python and the Pygame library, controlled entirely by an AI agent. The AI is trained to control the bird's movements, aiming to keep it flying through the pipes for as long as possible without crashing.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Game Mechanics](#game-mechanics)
- [AI Control](#ai-control)
- [Usage](#usage)
- [License](#license)

## Overview

In this project, Flappy Bird is powered by an AI model that learns and decides when to make the bird flap, avoiding pipes to maximize its score. Using Pygame for game development, this implementation serves as a fun demonstration of how AI can interact with real-time environments.

## Features

- **Classic Flappy Bird Gameplay**: Familiar gameplay with retro-styled graphics.
- **AI-Controlled Bird**: The AI agent learns to make decisions to keep the bird alive as long as possible.
- **Customizable Game Speed**: Adjust the game speed for training or demonstration purposes.
- **Real-Time Feedback**: Watch as the AI adapts and improves over time.

## Requirements

- Python 3.7 or later
- **Pygame** for game visuals and interactions
- **NEAT-Python** (or any other AI framework you’re using for training)

Install the required libraries:

```bash
pip install pygame
pip install neat-python  # If using NEAT for AI
```

## Installation

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/atharvapatil1210/flappy-bird-ai.git
    cd flappy-bird-ai
    ```

2. **Set Up Virtual Environment** (optional but recommended):
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install Dependencies**:
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the Game**:
    ```bash
    python flappy_bird_ai.py
    ```

## Game Mechanics

- **Objective**: Keep the bird alive by avoiding the pipes.
- **Scoring**: The score increases each time the bird successfully passes between two pipes.
- **End Condition**: The game ends if the bird collides with a pipe or falls to the ground.

## AI Control

The AI in this game uses [NEAT (NeuroEvolution of Augmenting Topologies)](https://neat-python.readthedocs.io/en/latest/) to control the bird. NEAT evolves neural networks over generations to find the optimal strategy for surviving the longest. The AI receives inputs such as the bird’s vertical position, distance to the next pipe, and the gap's position, allowing it to make informed decisions on when to flap.

### Key AI Components

- **Inputs**: Bird position, distance to pipes, pipe gap location.
- **Outputs**: Decision to flap or not.
- **Training**: The AI improves by evolving over many generations, gradually increasing its performance.

## Usage

1. **Running the Game**: Use `python flappy_bird_ai.py` to start the game. The AI will control the bird automatically.
2. **Adjusting Parameters**: If using NEAT, you can customize parameters in the `config-feedforward.txt` file to adjust AI learning rates, population size, etc.
3. **Viewing AI Progress**: As generations progress, observe how the AI learns to improve its survival time.


## Video-Demo
https://www.youtube.com/shorts/H9QTBYKPBUI

## License

This project is licensed under the MIT License.

