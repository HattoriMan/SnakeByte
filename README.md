# 🐍 SnakeByte - Terminal Snake Game

A feature-rich, interactive Snake game playable entirely in your terminal! Built with Python and the `curses` module, this game supports color display, multiple levels, power-ups, score tracking, key remapping, and pause functionality.

---

## 🎮 Features

- 🟩 **Colorful terminal graphics**
- 🧠 **Multiple difficulty levels**: Easy, Medium, Hard
- ⚡ **Power-ups** with dynamic effects:
  - `▲` Speed Up
  - `▼` Slow Down
  - `×` Shrink Snake
  - `+` Bonus Score
  - `-` Score Penalty
- ⌨️ **Customizable controls** via `key_config.json`
- ⏸️ **Pause menu** with instructions
- 💾 **High score tracking** per difficulty level
- 📜 **Gameplay logs** stored in JSON format
- 🔁 Seamless restart from game over

---

## 🚀 Getting Started

### 🔧 Prerequisites

- Python 3.7 or higher
- Works on Linux, macOS, and Windows (via `windows-curses` which would be installed when you install dependencies)

### 📦 Installation

1. **Clone the repository:**

```bash
git clone https://github.com/HattoriMan/SnakeByte
cd SnakeByte
```

Install dependencies with:

```bash
pip install -r requirements.txt
```

2. **Pip installation:**

You can install the package easily using pip:

```bash
pip install snakebyte
```

---

### ▶️ Run the Game

```bash
python game.py
````

Optional debug mode:

```bash
python game.py --debug
```

Or if installed via pip (from anywhere):

```bash
snake
```

---

## 🎮 Controls

| **Action**     | **Default Keys** |
| -------------- | ---------------- |
| Move Up        | `W` / `↑`        |
| Move Down      | `S` / `↓`        |
| Move Left      | `A` / `←`        |
| Move Right     | `D` / `→`        |
| Pause / Resume | `P`              |
| Instructions   | `I`              |
| Quit           | `Q` / `Esc`      |

---

### 🔧 Customize Keys

You can customize key bindings in the `key_config.json` file.

---

## 🗂️ Project Structure

```bash
.
├── game.py               # Main game logic
├── utils.py              # Game utilities
├── config.py             # Game configuration
├── key_config.py         # Key handling logic
├── key_config.json       # User-customizable key bindings
├── requirements.txt      # Python dependencies
├── logs/                 # Game logs and high scores(would be created once you run the game)
└── .gitignore            # Git exclusions
```

---

## 🧪 Levels & Gameplay

* **Levels**: Easy, Medium, Hard
* Snake wraps around screen edges
* Avoid biting your own body
* Collect food (`◉`) to grow and score
* Power-ups spawn periodically

---

## 📝 Logging

* Game history stored in: `logs/app.jsonl`
* High scores stored in: `logs/score.json`
* Error traces (if any): `logs/error_traceback.log`

---

## 🔜 Upcoming Features

✨ Planned enhancements:

* 🔊 Sound effects
* 💾 Save/Load game state
* 🧩 Challenges & achievements
* 🌐 Online high score leaderboard

---

## 📄 License

MIT License – use, modify, and distribute freely.


## 🙌 Acknowledgements

Thanks to the Python community and open-source contributors for the tools and inspiration that made this project possible. Inspired by the classic Snake game we all loved.

[![PyPI Downloads](https://static.pepy.tech/personalized-badge/snakebyte?period=total&units=INTERNATIONAL_SYSTEM&left_color=BLACK&right_color=GREEN&left_text=downloads)](https://pepy.tech/projects/snakebyte)
