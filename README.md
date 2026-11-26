# Pet Project Mini

**English** | [Tiếng Việt](README.vi.md)

A collection of small practice projects from my learning journey: three static front-end pages (HTML/CSS/JS) and a console Caro (Gomoku) game written in C++.

## Projects

| Folder | Project | Tech |
|---|---|---|
| [`FE_Project_1`](FE_Project_1) | Anime streaming landing page | HTML, CSS, Font Awesome, Google Fonts |
| [`FE_Project_2`](FE_Project_2) | "Softy Pinko" business landing page | HTML, CSS, Bootstrap 4, Font Awesome |
| [`FE_Project_3`](FE_Project_3) | "Vô Song Giáo" quiz Q&A lookup page | HTML, CSS, vanilla JavaScript |
| [`Console_GameCaro`](Console_GameCaro) | Caro (Gomoku) console game | C++, Win32 Console API, Visual Studio |

### 1. FE_Project_1 — Anime streaming page

A one-page layout for an anime streaming site, rebuilt from a design for front-end practice:

- Hero banner featuring *Demon Slayer*
- Genre cards (Shonen, Action, Fantasy, Romance, Comedy, Drama, Sci-Fi, Adventure)
- Sections for **Trending Shows**, **Continue Watching** and **Recently Released**
- Footer with link groups

Uses a CSS reset and a separate `base.css` / `styles.css` split.

### 2. FE_Project_2 — Softy Pinko landing page

A recreation of the *Softy Pinko* template (originally by TemplateMo), built with Bootstrap 4's grid:

- Hero banner, feature list and "work process" section
- Testimonials, pricing plans and blog entries
- Contact form and footer

### 3. FE_Project_3 — Vô Song Giáo Q&A lookup

A Vietnamese-language helper page for the "Vấn Đáp Tông Môn" quiz on a Chinese-animation (donghua) fan site:

- About **149 questions and answers** stored in `js.js`
- **Live search**: the table filters as you type in the search box
- Decorative Tết effects (fireworks GIF, falling apricot blossoms)

### 4. Console_GameCaro — Caro game in C++

A Caro (Gomoku) game that runs in the Windows console, built with object-oriented C++ (`_Board`, `_Game`, `_Point`, `_Common`, `_Play`).

**Features**

- 16 × 16 board drawn in the console
- Game modes: **Player vs Player** and **Player vs Computer**
- Computer opponent that scores every empty cell on attack and defense (horizontal, vertical and both diagonals) to pick its move; the code includes easy and hard scoring tables
- Win rule: exactly 5 in a row, not blocked at both ends (Vietnamese Caro rule)
- Score tracking across rounds, win/draw animations and a win sound
- **Save / load** games by file name (saved names are listed in `Name.txt`)

**Controls**

| Key | Action |
|---|---|
| `W` `A` `S` `D` | Move the cursor |
| `Enter` | Place a mark / choose a menu item |
| `L` | Save the game |
| `T` | Load a saved game |
| `Esc` | Back / exit |

**Build and run**

1. Open `Console_GameCaro/GameCaroConsole/GameCaroConsole.sln` in **Visual Studio 2022** (toolset v143).
2. Build and run (`Ctrl + F5`). Windows only, since the game uses `<Windows.h>`, `conio.h` and `winmm.lib` for sound.
3. Optional: put a `win.wav` file next to the executable to hear the win sound.

The project report (in Vietnamese) is in `Console_GameCaro/BaoCao.docx`.

## Running the front-end projects

No build step is needed. Clone the repo and open each project's `index.html` in a browser:

```bash
git clone https://github.com/thiennguyenk01/Pet_Project_Mini.git
cd Pet_Project_Mini
# then open FE_Project_1/index.html, FE_Project_2/index.html or FE_Project_3/index.html
```

An internet connection is needed to load fonts, icons and Bootstrap from their CDNs.

## Repository structure

```
Pet_Project_Mini/
├── FE_Project_1/          # Anime streaming page
│   ├── index.html
│   └── assets/ (css, images)
├── FE_Project_2/          # Softy Pinko landing page
│   ├── index.html
│   └── assets/ (css, images)
├── FE_Project_3/          # Vô Song Giáo Q&A lookup
│   ├── index.html
│   ├── style.css
│   ├── js.js
│   └── img/
└── Console_GameCaro/      # Caro game in C++
    ├── BaoCao.docx
    └── GameCaroConsole/   # Visual Studio solution
```

## Author

**Thien Nguyen** — [@thiennguyenk01](https://github.com/thiennguyenk01)

These are personal learning projects. Designs and content belong to their original owners.
