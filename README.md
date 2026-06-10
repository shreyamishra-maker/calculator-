# 🧮 Scientific Calculator

<div align="center">

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Offline](https://img.shields.io/badge/Offline-Supported-blueviolet?style=for-the-badge)
![Responsive](https://img.shields.io/badge/Responsive-Yes-00c896?style=for-the-badge)

A modern, responsive scientific calculator with advanced mathematical functions, calculation history, memory operations, keyboard support, and dark/light themes — all in a single HTML file with zero dependencies.

[Demo](#-screenshots) · [Installation](#-installation) · [Usage](#-usage) · [Contributing](#-contributing)

</div>

---

## ✨ Features

- ➕ **Basic Arithmetic** — Addition, subtraction, multiplication, division, percentage, sign toggle
- 🔬 **Scientific Functions** — sin, cos, tan (and inverses), log, ln, √, ∛, x², x³, xʸ, n!, |x|, 1/x
- 🧠 **Memory Operations** — MC, MR, MS, M+, M− with live memory indicator
- 📜 **Calculation History** — Scrollable panel, click any past result to reuse it, clear all
- ⌨️ **Keyboard Shortcuts** — Full keyboard support for fast input
- 🌗 **Dark / Light Mode** — Toggle between themes with a single click
- 📐 **DEG / RAD Toggle** — Switch angle mode directly from the display
- 📋 **Copy Result** — One-click copy of the current result to clipboard
- 🛡️ **Error Handling** — Graceful handling of division by zero, invalid inputs, and unclosed parentheses
- 📡 **Offline Support** — No CDN, no dependencies; works completely offline
- 📱 **Responsive Design** — Optimised for both desktop and mobile screens

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **HTML5** | Structure and semantic markup |
| **CSS3** | Glassmorphism UI, animations, theming via CSS variables |
| **Vanilla JavaScript** | All calculator logic, DOM manipulation, keyboard events |

No external libraries, frameworks, or build tools required.

---

## 📸 Screenshots

> **Add your screenshots here.**

| Dark Mode | Light Mode |
|---|---|
| ![Dark Mode Screenshot](screenshots/dark-mode.png) | ![Light Mode Screenshot](screenshots/light-mode.png) |

| Mobile View | History Panel |
|---|---|
| ![Mobile Screenshot](screenshots/mobile.png) | ![History Panel Screenshot](screenshots/history.png) |

---

## 🚀 Installation

Getting the calculator running locally takes less than a minute.

### Option 1 — Direct Open (Simplest)

```bash
# 1. Clone the repository
git clone https://github.com/your-username/scientific-calculator.git

# 2. Navigate into the project folder
cd scientific-calculator

# 3. Open the file in your browser
open scientific-calculator.html        # macOS
start scientific-calculator.html       # Windows
xdg-open scientific-calculator.html    # Linux
```

### Option 2 — Local Dev Server (Recommended for development)

```bash
# Using the VS Code Live Server extension
# Right-click scientific-calculator.html → "Open with Live Server"

# Or using Python's built-in server
python -m http.server 8000
# Then visit http://localhost:8000
```

### Option 3 — Deploy to GitHub Pages

```bash
# Push to your repo, then enable GitHub Pages:
# Settings → Pages → Source → main branch → / (root) → Save
# Your calculator will be live at: https://your-username.github.io/scientific-calculator
```

---

## 📖 Usage

### Basic Arithmetic

Click the number buttons or type on your keyboard to enter values. Use the operator buttons (`+`, `−`, `×`, `÷`) to chain operations, then press `=` or **Enter** to evaluate.

### Scientific Functions

Select a scientific function button **after** entering a number. The function is applied immediately to the current value:

| Button | Action | Example |
|---|---|---|
| `sin` / `cos` / `tan` | Trigonometric functions (respects DEG/RAD mode) | `sin(30)` → `0.5` |
| `sin⁻¹` / `cos⁻¹` / `tan⁻¹` | Inverse trigonometric | `sin⁻¹(0.5)` → `30` |
| `log` | Base-10 logarithm | `log(1000)` → `3` |
| `ln` | Natural logarithm | `ln(e)` → `1` |
| `√` | Square root | `√(9)` → `3` |
| `∛` | Cube root | `∛(27)` → `3` |
| `x²` | Square | `4 x²` → `16` |
| `x³` | Cube | `3 x³` → `27` |
| `xʸ` | Power (enter base, press `xʸ`, enter exponent, press `=`) | `2 xʸ 8` → `256` |
| `n!` | Factorial (integer values up to 170) | `5!` → `120` |
| `\|x\|` | Absolute value | `\|-9\|` → `9` |
| `1/x` | Multiplicative inverse | `1/x(4)` → `0.25` |
| `π` | Insert π (3.14159…) | — |
| `e` | Insert Euler's number (2.71828…) | — |

### Memory Operations

| Button | Description |
|---|---|
| **MS** | Store the current display value into memory |
| **MR** | Recall the stored memory value to the display |
| **M+** | Add the current display value to memory |
| **M−** | Subtract the current display value from memory |
| **MC** | Clear memory (the `M` indicator disappears) |

### Angle Mode

Tap the **DEG / RAD** badge on the display to toggle between degrees and radians. All trigonometric functions respect the active mode.

### History Panel

Every completed calculation is saved to the history panel on the right. Click any history entry to load that result back into the display. Use **Clear all** to reset the history.

---

## ⌨️ Keyboard Shortcuts

| Key | Function |
|---|---|
| `0` – `9` | Input numbers |
| `.` | Decimal point |
| `+` | Addition |
| `-` | Subtraction |
| `*` | Multiplication |
| `/` | Division |
| `%` | Percentage |
| `(` | Open parenthesis |
| `)` | Close parenthesis |
| `Enter` or `=` | Calculate result |
| `Backspace` | Delete last character |
| `Esc` or `Delete` | Clear all (AC) |

---

## 📁 Project Structure

```
scientific-calculator/
│
├── scientific-calculator.html   # Complete application (HTML + CSS + JS)
├── README.md                    # Project documentation
├── LICENSE                      # MIT License
│
└── screenshots/                 # App screenshots for README
    ├── dark-mode.png
    ├── light-mode.png
    ├── mobile.png
    └── history.png
```

Because the entire application lives in a single `.html` file, there are no build steps, no `node_modules`, and no configuration files needed.

---

## 🔮 Future Improvements

- [ ] 📊 **Graph Plotting** — Visualise functions like `sin(x)`, `x²`, and custom expressions
- [ ] 📐 **Unit Converter** — Length, mass, temperature, area, volume, and more
- [ ] 💱 **Currency Converter** — Live exchange rates via a free API
- [ ] 🧩 **Equation Solver** — Solve linear, quadratic, and polynomial equations step-by-step
- [ ] 💾 **Persistent History** — Save history to `localStorage` across sessions
- [ ] 🎨 **Custom Themes** — User-selectable accent colours
- [ ] ♿ **Accessibility** — Full ARIA labels and screen-reader support

---

## 🤝 Contributing

Contributions are welcome and appreciated! Here's how to get involved:

1. **Fork** the repository
2. **Create** a feature branch
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Commit** your changes with a clear message
   ```bash
   git commit -m "feat: add graph plotting support"
   ```
4. **Push** to your branch
   ```bash
   git push origin feature/your-feature-name
   ```
5. **Open a Pull Request** — describe what you changed and why

### Guidelines

- Keep all code in the single HTML file unless the scope genuinely requires a separate asset
- Write clean, commented JavaScript
- Test on both desktop and mobile before submitting
- Follow existing naming conventions and formatting

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2024 Your Name

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.
```

---

## 👤 Author

**Your Name**

- GitHub: [@your-username](https://github.com/shreyamishra-maker )


---

<div align="center">

If you found this project useful, please consider giving it a ⭐ on GitHub!

Made by shreya Mishra

</div>

