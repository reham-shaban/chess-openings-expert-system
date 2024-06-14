# Chess Opening Expert System

## Overview

The Chess Opening Expert System is an interactive engine that helps users explore and choose chess openings and moves. This engine uses an expert system based on the Experta framework to guide players through various chess openings, providing recommendations based on predefined certainty factors (CF).

## Features

- **Interactive Selection**: Users can choose to play as White or Black and then select from a list of openings tailored to their chosen color.
- **Opening Recommendations**: Openings are presented to help users make informed decisions.
- **Move Selection**: Users can choose from possible moves within an opening, with guidance provided for both White and Black moves.
- **Variants Handling**: The system supports handling variants within openings, allowing users to explore different branches of an opening.

## Structure

### Classes

- **Move**: Represents a single move in a chess opening, including fields for white's move, black's move, whether the move is a variant.
- **Branch**: Represents a branch of moves within an opening.
- **Opening**: Represents a chess opening, including its name, associated branches.
- **Path**: Keeps track of the moves played during the session.
- **ChessOpeningEngine**: The main engine that drives the interactive session, manages facts, rules, and user interactions.

## How to Run

1. **Clone the Repository**:
    ```sh
    git clone https://github.com/reham-shaban/chess-openings-expert-system
    cd chess-opening-expert-system
    ```

2. **Install Dependencies**:
    Ensure you have Python installed. Then install the required packages:
    ```sh
    pip install experta numpy
    ```

## Usage

1. **Start the Engine**:
    When you run the engine, you will be prompted to choose whether you want to play as White or Black.

2. **Choose an Opening**:
    Based on your chosen color, the system will list appropriate openings. Select an opening by typing its name.

3. **Follow the Moves**:
    The system will guide you through the moves of the chosen opening. For each move, you will be presented with possible options. You can choose a move by typing it in.

4. **Variants and Branches**:
    If the move has variants, you will be prompted to choose from the variant options. The system will update the branch accordingly.

## Example Interaction

```
Do you want to play as White or Black? white
You chose to play as white.

White Openings:
Ruy Lopez
Queen's Gambit
Choose an opening: Ruy Lopez

Ruy Lopez - Main Line:
0. e4 e5 
1. Nf3 Nc6 
2. Bb5 a6
3. Ba4 d6

Possible white moves: ['e4']
Choose white move: e4
Possible black moves: ['e5', 'e6']
Choose black move: e5
...
```
