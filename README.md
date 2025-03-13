# CoinFlip-Simulator

## Overview
CoinFlip-Simulator is a web-based simulation tool that demonstrates an interesting coin-flipping game between two players, **Alice** and **Bob**. In this simulation, a fair coin is flipped repeatedly, and points are awarded based on consecutive pairs:
- **Alice** receives a point for every occurrence of `HH` (heads followed by heads).
- **Bob** receives a point for every occurrence of `HT` (heads followed by tails).

## The Question
The underlying question driving this simulation is:

> **Flip a fair coin 100 times—it gives a sequence of heads (H) and tails (T). For each HH in the sequence, Alice gets a point; for each HT, Bob gets a point. For example, in the sequence `THHHT`, Alice gets 2 points and Bob gets 1 point. Who is most likely to win?**

The answer is **Bob**, because even though the expected scores for both players are identical, the higher variance in Alice's outcomes means that Bob wins more frequently with less extreme scores.

## Inspiration & Credit
This project was inspired by [Daniel Litt's post on X (Twitter)](https://x.com/littmath/status/1769044719034647001), which presented this puzzle and its counterintuitive result.

## Features
- **Interactive Simulation**:
  - **Simulate Game**: Run a single game with 20 coin flips.
  - **Simulate 100 Games**: Run a batch simulation to see historical trends.
- **Visualizations**:
  - **Sequence Canvas**: Displays the coin-flip sequence with overlapping red and blue bars indicating `HH` (red, below the text) and `HT` (blue, above the text) events.
  - **Current Game Chart**: A bar chart showing the scores for the current game for both Alice and Bob.
  - **Score Difference Frequency Chart**: A histogram showing the frequency distribution of the score differences (Alice's score minus Bob's score) over all games.
  - **Score Frequency Chart**: A histogram displaying the frequency of scores (from 0 to 19) for both players over all games.
- **Historical Statistics**: Displays average scores, standard deviations, win counts, and tie counts across all simulated games.

## Setup & Usage
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/CoinFlip-Simulator.git
   cd CoinFlip-Simulator
   ```
2. **Open the Project**  
   Simply open the `index.html` file in your web browser.
3. **Run Simulations**  
   Click **Simulate Game** to run an individual game.

   Click **Simulate 100 Games** to run a batch simulation and observe how the historical statistics and visualizations evolve.

## License
This project is open source and available under the [MIT License](LICENSE).