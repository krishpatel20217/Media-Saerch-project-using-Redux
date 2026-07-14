# 🔎 Media Search App

![React](https://img.shields.io/badge/React-19-61DAFB?logo=react&logoColor=white)
![Redux Toolkit](https://img.shields.io/badge/Redux%20Toolkit-State-764ABC?logo=redux&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-Build-646CFF?logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-4-06B6D4?logo=tailwindcss&logoColor=white)

A modern media search application built with **React**, **Redux Toolkit**, **Vite**, and **Tailwind CSS**. The application lets users search **images from Unsplash** and **videos from Pexels**, then save their favorite media into a personal collection managed through Redux.

> This project was built to practice API integration, global state management with Redux Toolkit, routing, and building a responsive React application.

---

# ✨ Features

- 🔍 Search images using the Unsplash API
- 🎥 Search videos using the Pexels API
- ❤️ Save favorite media to a personal collection
- 🗑️ Remove individual items or clear the collection
- ⚡ Global state management with Redux Toolkit
- 🔄 Client-side routing using React Router
- 🔔 Toast notifications for user actions
- 📱 Responsive UI
- 🚀 Fast development with Vite

---

# 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | React 19 |
| State Management | Redux Toolkit |
| Routing | React Router DOM |
| HTTP Client | Axios |
| Styling | Tailwind CSS 4 |
| Notifications | React Toastify |
| Build Tool | Vite |
| APIs | Unsplash & Pexels |

---

# 🏗️ Project Architecture

```text
User
 │
 ▼
Search Bar
 │
 ▼
Redux searchSlice
 │
 ▼
Axios Request
 ├──────────────┐
 ▼              ▼
Unsplash     Pexels
 │              │
 └──────┬───────┘
        ▼
Result Grid
        │
        ▼
Collection Slice
        │
        ▼
Collection Page
```

---

# 📂 Folder Structure

```text
src/
├── api/
├── components/
│   ├── CollectionCard.jsx
│   ├── Navbar.jsx
│   ├── ResultCard.jsx
│   ├── ResultGrid.jsx
│   ├── SearchBar.jsx
│   └── Tabs.jsx
├── pages/
│   ├── HomePage.jsx
│   └── CollectionPage.jsx
├── redux/
│   ├── features/
│   │   ├── searchSlice.js
│   │   └── collectionSlice.js
│   └── store.js
├── App.jsx
└── main.jsx
```

---

# 🔄 Application Flow

1. User enters a search query.
2. Redux stores the query.
3. Axios requests data from Unsplash or Pexels.
4. Results are displayed in a responsive grid.
5. Users can save media to their collection.
6. Collection is managed globally through Redux Toolkit.

---

# 📦 Redux Store

- **searchSlice** – stores current search query, active media type and search results.
- **collectionSlice** – manages the user's saved media collection.
- **store.js** – configures the Redux store.

---

# 🌐 APIs

## Unsplash
Used for image search.

## Pexels
Used for video search.

---

# ⚙️ Environment Variables

Create a `.env` file.

```env
VITE_UNSPLASH_KEY=your_unsplash_api_key
VITE_PEXELS_KEY=your_pexels_api_key
```

---

# 🚀 Installation

```bash
git clone https://github.com/krishpatel20217/Media-Saerch-project-using-Redux.git

cd Media-Saerch-project-using-Redux

npm install

npm run dev
```

---


# 🚀 Future Improvements

- Infinite scrolling
- Download media
- Search history
- Debounced search
- Pagination
- Dark mode
- Advanced filters
- User authentication
- Recently searched items

---

# 🤝 Contributing

Contributions are welcome. Fork the repository, create a feature branch, commit your changes, and open a Pull Request.

---

# 📄 License

MIT License.

---

# 👨‍💻 Author

**Krish Patel**

If you found this project useful, consider giving it a ⭐ on GitHub.
