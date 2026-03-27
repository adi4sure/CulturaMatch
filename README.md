# CulturaMatch 🌍

A cultural exchange platform connecting people worldwide for skill sharing, language learning, and cultural interaction — powered by **AI matching** using Neural Networks & Fuzzy Logic.

## Architecture

```
┌──────────────────┐     ┌─────────────────┐     ┌──────────────────────┐
│   React + Vite   │────▶│  Node.js/Express│────▶│  Python Flask AI     │
│   Frontend       │ API │  Backend        │ API │  Matching Service    │
│   (port 5173)    │     │  (port 5000)    │     │  (port 5001)         │
└──────────────────┘     └─────────────────┘     └──────────────────────┘
                              │                       │
                              ▼                       ▼
                         JSON File Storage       Neural Network +
                         (users, chats, etc.)    Fuzzy Logic Engine
```

## Features

- **AI-Powered Matching** — Fuzzy logic + neural network for intelligent cultural exchange partner matching
- **Skill Sharing** — Share and learn skills like music, cooking, coding, and more
- **Language Exchange** — Find native speakers and practice languages together
- **Real-time Chat** — Instant messaging with your matches
- **Virtual Meetups** — Schedule and manage cultural exchange sessions
- **Feedback System** — Rate interactions to improve AI recommendations

## Quick Start

### Prerequisites
- Node.js 18+
- Python 3.9+ (optional, for AI service)

### Install & Run

```bash
# 1. Install dependencies
cd frontend && npm install
cd ../backend && npm install

# 2. Start backend (Terminal 1)
cd backend && npm run dev

# 3. Start frontend (Terminal 2)
cd frontend && npm run dev

# 4. (Optional) Start AI service (Terminal 3)
cd ai-service
pip install -r requirements.txt
python app.py
```

Open **http://localhost:5173** in your browser.

### Demo Users
The app comes with 6 pre-seeded demo users from Japan, Brazil, India, Germany, Morocco, and South Korea. Register a new account to see AI-matching in action!

## Tech Stack

| Layer    | Technology                           |
|----------|--------------------------------------|
| Frontend | React 18, Vite, React Router, Lucide |
| Backend  | Node.js, Express, JWT, bcrypt        |
| AI       | Python Flask, NumPy, Fuzzy Logic     |
| Storage  | JSON files (zero-config)             |
| Design   | Dark glassmorphism, Inter + Outfit   |

## AI Matching Pipeline

1. **Fuzzy Logic Engine** — Triangular & trapezoidal membership functions score compatibility across skill overlap, language similarity, cultural interest alignment, and timezone proximity
2. **Neural Network** — Feedforward network (4→8→1) trained on user feedback to personalize match quality
3. **Combined Score** — Weighted blend: 60% fuzzy + 40% neural prediction

## License

MIT
