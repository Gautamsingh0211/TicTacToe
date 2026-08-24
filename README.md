# 🎮 Tic Tac Toe — React

A simple and interactive **Tic Tac Toe game** built using **React.js**.

This project demonstrates fundamental React concepts such as **components, state management, event handling, conditional rendering, and dynamic UI updates**.

## 🚀 Features

* 🎯 Two-player Tic Tac Toe game
* ❌ Player X and ⭕ Player O turns
* 🏆 Automatically detects the winner
* 🤝 Detects draw/tie games
* 🔄 Reset/New Game functionality
* ⚡ Fast and responsive UI
* 🧩 Built with reusable React components

## 🛠️ Tech Stack

* **React.js**
* **JavaScript (ES6+)**
* **CSS3**
* **Vite**
* **React Hooks**

  * `useState`
  * `useRef`
  
## 📂 Project Structure

```text
tic-tac-toe/
├── public/
├── src/
│   ├── assets/
│   │   ├── circle.png
│   │   └── cross.png
│   ├── components/
│   ├── App.jsx
│   ├── TicTacToe.jsx
│   ├── TicTacToe.css
│   ├── main.jsx
│   └── index.css
├── package.json
├── package-lock.json
└── README.md
```

> The exact folder structure may vary depending on your project setup.

## ⚙️ Installation

### 1. Clone the repository

```bash
git clone <your-repository-url>
```

### 2. Navigate to the project directory

```bash
cd tic-tac-toe
```

### 3. Install dependencies

```bash
npm install
```

### 4. Start the development server

```bash
npm run dev
```

The application will be available at the local URL provided by Vite, usually:

```text
http://localhost:5173
```

## 🎮 How to Play

1. The game starts with **Player X**.
2. Players take turns clicking on an empty cell.
3. The first player to get **three of their symbols in a row** wins.
4. A winning combination can be:

   * Horizontal
   * Vertical
   * Diagonal
5. If all cells are filled and nobody wins, the game ends in a **draw**.
6. Click **Reset** or **New Game** to start another round.

## 🧠 React Concepts Used

### `useState`

The game uses React's `useState` hook to keep track of things such as:

* Current player's turn
* Board values
* Whether the game is locked
* Winner/game status

Example:

```jsx
const [count, setCount] = useState(0);
const [lock, setLock] = useState(false);
```

### Event Handling

Click events are handled to determine which cell the player selected.

```jsx
function toggle(index) {
    // Update the selected cell
}
```

### Conditional Rendering

The UI changes depending on the current game state, such as displaying the winner or allowing the player to continue playing.

## 🏆 Winning Conditions

There are **8 possible winning combinations**:

```text
0  1  2
3  4  5
6  7  8
```

Winning combinations:

```javascript
[
    [0, 1, 2],
    [3, 4, 5],
    [6, 7, 8],
    [0, 3, 6],
    [1, 4, 7],
    [2, 5, 8],
    [0, 4, 8],
    [2, 4, 6]
]
```

The game checks these combinations after every move to determine whether a player has won.

## 📸 Preview

<img width="1157" height="857" alt="image" src="https://github.com/user-attachments/assets/0e2406dd-a75d-44ed-a577-4f79a205b2e3" />


```markdown
![Tic Tac Toe Preview](./screenshot.png)
```

## 🔮 Future Improvements

Some possible improvements:

* [ ] Add single-player mode against the computer
* [ ] Add difficulty levels
* [ ] Add score tracking
* [ ] Add player name customization
* [ ] Add sound effects
* [ ] Add animations
* [ ] Add dark/light mode
* [ ] Make the game fully responsive for mobile devices

## 🤝 Contributing

Contributions are welcome!

1. Fork the repository.
2. Create a new branch.

```bash
git checkout -b feature/new-feature
```

3. Make your changes.
4. Commit your changes.

```bash
git commit -m "Add new feature"
```

5. Push the branch.

```bash
git push origin feature/new-feature
```

6. Open a Pull Request.

## 📄 License

This project is open source and available under the **MIT License**.

---

⭐ If you found this project useful, consider giving the repository a star!
