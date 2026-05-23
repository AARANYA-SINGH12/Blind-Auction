# 🔨 Blind Auction

A command-line Blind Auction program built with Python where multiple bidders can secretly place their bids and the highest bidder is announced at the end.

---

## 📖 About

In a blind auction, bidders place their bids without knowing what others have offered. This program simulates that experience in a terminal — each bidder enters their name and bid privately, the screen clears between bidders to keep bids hidden, and the winner is revealed once all bids are in.

---

## ✨ Features

- **Multiple bidder support** — any number of participants can place bids in a single session
- **Secret bidding** — screen clears between each bidder so no one can see others' bids
- **Automatic winner detection** — finds and announces the highest bidder at the end
- **ASCII art logo** displayed on launch via `art.py`
- **Simple and clean flow** — prompts guide each bidder step by step

---

## 🖥️ Prerequisites

- Python 3.x

No external libraries required.

---

## 🚀 Getting Started

1. **Clone the repository:**
```bash
   git clone https://github.com/AARANYA-SINGH12/Blind-Auction.git
   cd Blind-Auction
```

2. **Run the program:**
```bash
   python auction.py
```

---

## 🕹️ How to Use

1. The first bidder enters their **name** and their **bid amount**
2. When asked if there are other bidders, type `yes` — the screen clears for the next person
3. Each subsequent bidder enters their name and bid privately
4. When the last bidder types `no`, the program announces the **winner and winning bid**

**Example:**
```
What's your name?: Alice
What's your bid?: $150
Are there any other bidders? Type 'yes' or 'no'.
yes

What's your name?: Bob
What's your bid?: $200
Are there any other bidders? Type 'yes' or 'no'.
no

The winner is Bob with a bid of $200.
```

---

## 📁 Project Structure

```
Blind-Auction/
│
├── auction.py     # Main program logic
└── art.py         # ASCII art logo displayed on launch
```

---

## 🧠 Concepts Used

- Dictionaries (storing name-bid pairs)
- Functions
- Loops (`while`)
- Conditional statements (`if/elif`)
- Screen clearing using repeated newlines

---

## 🐛 Known Limitations

- Entering a non-integer value for the bid will cause a crash — no input validation is implemented
- Screen clearing uses `print("\n" * 100)` which may not fully clear the terminal on all systems; `os.system('clear')` or `os.system('cls')` would be more reliable

---

## 📜 License

This project is open-source and free to use for personal and educational purposes.
