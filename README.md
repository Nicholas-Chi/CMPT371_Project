# CMPT 371: Deny and Conquer

Deny and Conquer is a multiplayer drawing game developed in Python using Pygame and TCP/IP socket communication. Players connect to a host and compete to claim squares on a shared grid by drawing over them. A square is claimed when at least 50% of its area is covered by a player's colour. Once all squares have been filled, a leaderboard displays the final results.

## Requirements

Before running the game, make sure you have installed:

- **Python 3** – [Download Python](https://www.python.org/downloads/)
- **Pygame** – The library used to handle graphics and gameplay

## Installation

1. Download or clone this repository.
2. Extract the project files if downloaded as a ZIP archive.
3. Install Python 3 if it is not already installed.
4. Install Pygame by opening a terminal in the project folder and running:

   ```bash
   python -m pip install pygame
   ```

   If `python` is not recognized, try `python3` or `py` instead.

## How to Run

1. Open a terminal or command prompt in the project directory.
2. Start the game by running:

   ```bash
   python main.py
   ```

3. Choose to host a new game or join an existing game by entering the host's IP address.
4. If hosting a game for players on other networks, configure your router's port forwarding for the port used by the game. Ensure your firewall allows the connection as well.
5. Play until all squares on the grid have been claimed.
6. View the leaderboard to see the final results.
7. Close the game when finished. Run `main.py` again to start another session.

## Multiplayer Setup

- **Hosting:** One player starts the game as the host and shares their IP address with other players.
- **Joining:** Other players enter the host's IP address to connect to the game.
- **Same network:** Players on the same local network can generally connect using the host's local IP address.
- **Different networks:** The host may need to configure port forwarding and firewall rules to allow incoming connections.

Make sure all players can reach the host on the port configured by the game.

## Technologies Used

- Python 3
- Pygame
- TCP/IP sockets
- Multithreading

## Notes

- Keep the game running on the host computer while other players are connected.
- Start a new session by running `main.py` again after closing the previous game.
