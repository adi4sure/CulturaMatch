<div align="center">

# 🌍 CulturaMatch

### *Connect Cultures, Share Skills, Grow Together*

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![React](https://img.shields.io/badge/React-18-61DAFB?logo=react&logoColor=white)](https://react.dev/)
[![Node.js](https://img.shields.io/badge/Node.js-18+-339933?logo=node.js&logoColor=white)](https://nodejs.org/)
[![Python](https://img.shields.io/badge/Python-3.9+-3776AB?logo=python&logoColor=white)](https://python.org/)
[![Vite](https://img.shields.io/badge/Vite-6-646CFF?logo=vite&logoColor=white)](https://vitejs.dev/)

A cultural exchange platform powered by **AI matching** (Neural Networks & Fuzzy Logic) that connects people worldwide for skill sharing, language learning, and cultural interaction.

<br>

<img src="screenshots/landing_page.png" alt="CulturaMatch Landing Page" width="90%">

</div>

---

## 📸 Screenshots

### Landing Page
<div align="center">
<img src="screenshots/landing_page.png" alt="Landing Page" width="90%">
</div>

---

### Registration (3-Step Flow)
<div align="center">
<table>
  <tr>
    <td align="center"><strong>Step 1 — Personal Details</strong></td>
    <td align="center"><strong>Step 2 — Skills & Languages</strong></td>
  </tr>
  <tr>
    <td><img src="screenshots/registration_step1.png" alt="Registration Step 1" width="100%"></td>
    <td><img src="screenshots/registration_step2.png" alt="Registration Step 2" width="100%"></td>
  </tr>
</table>
</div>

---

### Login
<div align="center">
<img src="screenshots/login_page.png" alt="Login Page" width="90%">
</div>

---

### Dashboard
<div align="center">
<img src="screenshots/dashboard.png" alt="Dashboard" width="90%">
</div>

---

### AI-Powered Discover Page
<div align="center">
<img src="screenshots/discover_matches.png" alt="Discover Matches" width="90%">
</div>

---

### Chat
<div align="center">
<img src="screenshots/chat_page.png" alt="Chat Page" width="90%">
</div>

---

### Profile
<div align="center">
<img src="screenshots/profile_page.png" alt="Profile Page" width="90%">
</div>

---

### Virtual Meetups
<div align="center">
<img src="screenshots/meetups_page.png" alt="Meetups Page" width="90%">
</div>

---

## 🛠️ Technologies Used

### Frontend
- **React 18** — Component-based UI library
- **Vite 6** — Fast build tool and dev server
- **React Router** — Client-side routing
- **Lucide React** — Icon library
- **CSS3** — Dark glassmorphism design with custom animations
- **Google Fonts** — Inter & Outfit typography

### Backend
- **Node.js** — JavaScript runtime
- **Express.js** — Web framework for REST API
- **JSON Web Tokens (JWT)** — Authentication
- **bcrypt** — Password hashing
- **CORS** — Cross-origin resource sharing
- **JSON File Storage** — Zero-config data persistence

### AI Matching Service
- **Python 3.9+** — Programming language
- **Flask** — Lightweight web framework
- **NumPy** — Numerical computing
- **Fuzzy Logic** — Triangular & trapezoidal membership functions for compatibility scoring
- **Neural Network** — Feedforward network (4→8→1) trained on user feedback

---

## 📖 How to Use — Step by Step

### Step 1: Clone & Install

```bash
git clone https://github.com/adi4sure/CulturaMatch.git
cd CulturaMatch

# Install frontend
cd frontend && npm install

# Install backend
cd ../backend && npm install

# (Optional) Install AI service
cd ../ai-service && pip install -r requirements.txt
```

### Step 2: Start the Application

Open **3 terminals** and run:

```bash
# Terminal 1 — Start Backend (port 5000)
cd backend && npm run dev

# Terminal 2 — Start Frontend (port 5173)
cd frontend && npm run dev

# Terminal 3 — Start AI Service (port 5001) [Optional]
cd ai-service && python app.py
```

### Step 3: Open in Browser

Go to **http://localhost:5173**

### Step 4: Register Your Account

1. Click **"Get Started"** on the landing page
2. **Step 1** — Enter your name, email, password, and country
3. **Step 2** — Select skills you can teach and languages you speak
4. **Step 3** — Choose your cultural interests and write a short bio
5. Click **"Create Account"**

### Step 5: Explore the Dashboard

After registration you'll land on your **Dashboard** showing:
- Total matches found, conversations, meetups, and feedback stats
- Your recent AI matches with compatibility scores
- Your profile summary

### Step 6: Discover Matches

Go to the **Discover** page to see AI-matched cultural exchange partners ranked by compatibility percentage. Each card shows the user's country, bio, skills, languages, and interests.

### Step 7: Start Chatting

Open the **Chat** page to message your matches. Select a contact from the sidebar and start a conversation.

### Step 8: Schedule Meetups

Visit the **Meetups** page to schedule virtual cultural exchange sessions with your partners.

### Step 9: Manage Your Profile

Go to **Profile** to view and edit your skills, languages, interests, and bio.

---

## 🏗️ Architecture

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

---

## 🧠 AI Matching Pipeline

| Stage | Method | Details |
|-------|--------|---------|
| **Fuzzy Logic** | Membership functions | Scores skill overlap, language similarity, interest alignment, timezone proximity |
| **Neural Network** | Feedforward (4→8→1) | Learns from user feedback to personalize match quality |
| **Combined Score** | Weighted blend | 60% fuzzy + 40% neural = final match ranking |

---

## 👥 Demo Users

The app includes **6 pre-seeded users** for testing:

| Name | Country | Skills | Languages |
|------|---------|--------|-----------|
| 🇯🇵 Aiko Tanaka | Japan | Calligraphy, Cooking, Martial Arts | Japanese, English |
| 🇧🇷 Carlos Rivera | Brazil | Music, Dance, Cooking, Photography | Portuguese, Spanish, English |
| 🇮🇳 Priya Sharma | India | Yoga, Dance, Cooking, Painting | Hindi, English, Sanskrit |
| 🇩🇪 Emma Müller | Germany | Music, Writing, Philosophy | German, English, French |
| 🇲🇦 Fatima Al-Hassan | Morocco | Cooking, Pottery, Calligraphy | Arabic, French, English |
| 🇰🇷 Yuki Park | South Korea | Film Making, Music, Coding | Korean, English, Japanese |

---

## 📁 Project Structure

```
CulturaMatch/
├── frontend/                # React + Vite frontend
│   ├── src/
│   │   ├── pages/           # All page components
│   │   ├── App.jsx          # Routing + auth context
│   │   └── index.css        # Design system
│   └── index.html
├── backend/                 # Node.js + Express backend
│   ├── server.js            # REST API
│   └── data/                # JSON file storage
├── ai-service/              # Python Flask AI service
│   ├── app.py               # Fuzzy logic + neural network
│   └── requirements.txt
├── screenshots/             # Interface screenshots
└── README.md
```

---

## 📄 License

MIT License — see [LICENSE](LICENSE) for details.

---

<div align="center">

**Built with ❤️ for cultural exchange and global connection**

</div>
