# 🎟️ Lottery Game

A simple, interactive lottery game built with React. Buy a ticket, get three random numbers, and see if their sum matches the winning number!

## Demo

> [Link](https://lottery-game-eosin-eight.vercel.app/)

## ✨ Features

- 🎲 Randomly generated ticket numbers on each draw
- 🏆 Automatic win detection based on a configurable winning sum
- 🔁 "Buy New Ticket" button to redraw instantly
- 🎨 Clean, modern UI with a purple-accent theme
- ⚙️ Configurable ticket size (`n`) and winning sum via props

## 🛠️ Tech Stack

- **React** (with Hooks – `useState`)
- **Vite** – fast dev server and build tool
- **CSS3** – custom styling, no external UI libraries

## 📂 Project Structure

```
src/
├── App.jsx
├── Lottery.jsx       # Main game logic & state
├── Lottery.css
├── Ticket.jsx         # Renders the list of ticket numbers
├── Ticket.css
├── TicketNum.jsx      # Renders a single number
├── TicketNum.css
├── helper.js           # genTicket() and sum() utility functions
└── index.css            # Global page styling
```

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v16 or higher recommended)
- npm (comes with Node.js)

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/ronit-patidar/lottery-game.git
   cd lottery-game
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Start the development server
   ```bash
   npm run dev
   ```

4. Open your browser and visit the local URL shown in the terminal (typically `http://localhost:5173`)

## 🎮 How to Play

1. A ticket with random numbers is generated automatically when the page loads.
2. Click **Buy New Ticket** to generate a new set of numbers.
3. If the sum of the numbers equals the winning sum, you'll see a congratulations message!

## ⚙️ Configuration

The `Lottery` component accepts two optional props:

```jsx
<Lottery n={3} winningSum={15} />
```

| Prop         | Type   | Default | Description                              |
|--------------|--------|---------|------------------------------------------|
| `n`          | number | `3`     | Number of digits/numbers on the ticket   |
| `winningSum` | number | `15`    | The sum required to win                  |

## 📌 Future Improvements

- [ ] Add animation when a new ticket is drawn
- [ ] Add a pulse/confetti effect on winning
- [ ] Track and display ticket purchase history
- [ ] Add sound effects

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 👤 Author

**Ronit Patidar**
GitHub: [@ronit-patidar](https://github.com/ronit-patidar)
