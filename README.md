# Flappy Bird ML

This project is an implementation of the Flappy Bird game using machine learning with the NEAT algorithm. The game is built using Pygame, and the NEAT algorithm is used to train a neural network to play the game.

## Requirements

- Python 3.x
- Pygame
- NEAT-Python
- Pickle

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/LTPPPP/Flappy-bird-auto.git
   ```
2. Navigate to the project directory:
   ```sh
   cd flappy-bird-ML
   ```
3. Install the required packages:
   ```sh
   pip install pygame neat-python
   ```

## Running the Game

To run the game, execute the following command:

```sh
python flappy_bird.py
```

## Project Structure

- `flappy_bird.py`: Main script to run the game.
- `config.txt`: Configuration file for the NEAT algorithm.
- `imgs/`: Directory containing game images.
- `README.md`: Project documentation.

## How It Works

The game uses the NEAT (NeuroEvolution of Augmenting Topologies) algorithm to evolve a neural network that can play Flappy Bird. The neural network is trained over multiple generations to improve its performance.

### Key Classes and Functions

- `Bird`: Represents the bird in the game.
- `Pipe`: Represents the pipes in the game.
- `Base`: Represents the moving floor of the game.
- `blitRotateCenter`: Rotates an image and blits it to the screen.
- `draw_window`: Draws the game window.
- `eval_genomes`: Evaluates the genomes in the population.
- `run`: Runs the NEAT algorithm.

## Training the Neural Network

The neural network is trained using the NEAT algorithm. The training process involves the following steps:

1. Initialize the population.
2. Evaluate the fitness of each genome.
3. Select the best genomes to reproduce.
4. Apply crossover and mutation to create a new generation.
5. Repeat the process for a specified number of generations.

The fitness of a genome is determined by how well the bird it controls performs in the game. The longer the bird survives and the more pipes it passes, the higher its fitness score.

## Saving the Best Model

If the neural network achieves a score greater than 20, the best model is saved to a file named `best.pickle`.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [Pygame](https://www.pygame.org/)
- [NEAT-Python](https://neat-python.readthedocs.io/en/latest/)
- [Flappy Bird](https://flappybird.io/)

Feel free to contribute to this project by opening issues or submitting pull requests.
