# 🃏 Blackjack Card Game (Python CLI Version)
This is a simple, terminal-based implementation of the classic **Blackjack** game written in **Python**. The goal? Beat the dealer by getting your hand as close to 21 as possible **without going over**.



## How to Run

Make sure you have Python installed on your system (version 3+ recommended).

1. Clone this repository or copy the code into a Python file:
    ```bash
    git clone <your-repo-url>
    cd blackjack-card-game
    ```

2. Run the game:
    ```bash
    python blackjack.py
    ```

## How to Play Blackjack (for Beginners)

### Objective
- Get a hand total **closer to 21 than the dealer**.
- If you go over 21, that’s a **bust**, and you automatically lose.

## Card Values
- Number cards (2-10): Face value
- Face cards (J, Q, K): 10 points
- Ace (A): **11 points**, but switches to **1** if counting it as 11 would bust your hand.

## Game Flow

1. You’ll be asked **how many games** you want to play.
2. Each game starts by dealing **2 cards to you and 2 to the dealer** (1 hidden).
3. You can choose to:
   - **Hit (h)** → Get another card.
   - **Stand (s)** → Keep your current hand.
4. If your total goes over 21, you **bust** and lose.
5. Once you stand, the **dealer reveals their hand** and draws until reaching **17 or more**.
6. Winner is decided:
   - Closest to 21 wins.
   - Equal totals = Tie
   - Blackjack (an Ace + 10/J/Q/K) right away = Instant win.

## Features

- Multiple game rounds.
- Realistic card dealing with shuffling.
- Blackjack detection.
- Dealer logic that follows official rules.
- Simple CLI-based UI.

## Code Structure

- `Deck`: Creates and shuffles a 52-card deck.
- `Hand`: Manages player/dealer hands, calculating values and checking for blackjack.
- `Game`: Controls the full game loop, from dealing cards to declaring the winner.

## Example Gameplay
How many games do you want to play? 1

Game 1 of 1

Your hand:
10 of hearts
A of spades
Value: 21

Dealer's
hidden
8 of clubs

Player has blackjack. You win!
Thanks for playing!

