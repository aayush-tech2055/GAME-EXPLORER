# 🎮 Game Explorer

A responsive web application that lets users browse, search, filter, and sort video games using the **RAWG Video Games API**. Built with vanilla JavaScript, HTML, and CSS as part of a web development project.

---

## 📌 Project Purpose

Game Explorer allows users to discover detailed information about thousands of video games from around the world. Users can search by game title, filter by genre, platform, or rating, sort by various attributes, view game screenshots, and save games to a personal wishlist — all in a clean, responsive interface.

---

## 🌐 API Used

**RAWG Video Games API**
- Base URL: `https://api.rawg.io/api/`
- Free tier API key required → [Get your key here](https://rawg.io/apidocs)
- Key endpoints used:
  - `GET /games` — Browse and search all games
  - `GET /games/{id}` — Fetch full game details
  - `GET /games/{id}/screenshots` — Fetch game screenshots
  - `GET /genres` — List all available genres
  - `GET /platforms` — List all available platforms

---

## ✨ Planned Features

### Core Features (Milestones 2 & 3)
- 🔍 **Search** — Search games by title using a live search bar (with debouncing)
- 🎛️ **Filter** — Filter games by:
  - Genre (Action, RPG, Strategy, Sports, Puzzle, etc.)
  - Platform (PC, PlayStation, Xbox, Nintendo Switch)
  - Rating range (e.g., 3.0+ to 5.0)
- 🔃 **Sort** — Sort results by:
  - Release date (newest / oldest)
  - Rating (highest / lowest)
  - Name (A–Z / Z–A)
- 🖼️ **Screenshots Viewer** — View game screenshots in a modal/lightbox on click
- ❤️ **Wishlist** — Add/remove games to a personal wishlist (stored in Local Storage)
- 🌙 **Dark / Light Mode** — Theme toggle with preference saved in Local Storage
- 📄 **Game Detail View** — Click a game card to see full details (description, platforms, rating, genres, release date)

### Bonus Features
- ⏱️ **Debouncing** on search input to reduce unnecessary API calls
- 📦 **Pagination** to manage large lists of games
- 🔄 **Loading Indicators** while data is being fetched
- 💾 **Local Storage** for wishlist and dark mode preference

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| HTML5 | Page structure and markup |
| CSS3 | Styling and responsive layout |
| JavaScript (ES6+) | Logic, API calls, DOM manipulation |
| Fetch API | Fetching data from RAWG API |
| Array HOFs | `filter()`, `sort()`, `map()`, `find()` for data operations |
| Local Storage | Persisting wishlist and theme preference |

> 💡 No frameworks used — pure vanilla JavaScript.

---

## 📁 Project Structure

```
game-explorer/
│
├── index.html          # Main HTML file
├── style.css           # Stylesheet (responsive design)
├── app.js              # Main JavaScript file
│
├── js/
│   ├── api.js          # API fetch logic
│   ├── render.js       # UI rendering functions
│   ├── filter.js       # Search, filter, sort logic (HOFs)
│   └── storage.js      # Local storage utilities
│
└── README.md           # Project documentation
```

---

## 🚀 How to Run the Project

### Prerequisites
- A modern web browser (Chrome, Firefox, Edge)
- A free API key from [https://rawg.io/apidocs](https://rawg.io/apidocs)

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/aayush-tech2055/game-explorer.git
   cd game-explorer
   ```

2. **Add your API key**

   Open `js/api.js` and replace the placeholder with your key:
   ```javascript
   const API_KEY = "your_api_key_here";
   ```

3. **Open in browser**

   Simply open `index.html` in your browser — no build tools or server needed.

   Or use VS Code's **Live Server** extension for a better experience.

---

## 📅 Project Milestones

| Milestone | Description | Deadline |
|---|---|---|
| Milestone 1 | Project setup, idea selection, README | 23rd March |
| Milestone 2 | API integration, data display, responsiveness | 1st April |
| Milestone 3 | Search, filter, sort, dark mode, wishlist | 8th April |
| Milestone 4 | Final cleanup, deployment, documentation | 10th April |

---

## 🌍 Deployment

The project will be deployed using **GitHub Pages** (or Netlify).

Live link will be added here after deployment.

---

## 👨‍💻 Author

**Aayush Ruparelia**
- GitHub: [@aayush-tech2055](https://github.com/aayush-tech2055)

---

## 📄 License

This project is for educational purposes only.
