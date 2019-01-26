# lc0-tui
Terminal based user interface for lc0
This will run on a tiny instance (free) on Google Cloud Platform or a Raspberry Pi

Use small weights files e.g. from https://github.com/dkappe/leela-chess-weights/releases

## Basic instructions

```
git clone https://github.com/gsobala/lc0-tui
cd lc0-tui
pip3 install python-chess
```

Edit main.py CONFIG section to reflect location of lc0 and weights file
also optionally change the time control

```
python3 main.py
```

* The TUI remembers the last position played so you can leave a game and carry on.
* The keys for each setting are shown on the interface.
* Shift-E to start and stop the engine.
* Shift-T to start and stop the clocks.
* Moves are entered as e.g. e2e4 followed by (Enter) key.
* To change Leela sides, switch the 'timed' and 'infinite' statuses for White and Black.
* Control-C to quit the program

``rm data/state.bin`` to delete the state file and reset to a new game

