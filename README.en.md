# 🎮 Interactive Pokédex

<div align="center">
  <img src="https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D" alt="Vue.js">
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/Vite-B73E9E?style=for-the-badge&logo=vite&logoColor=FFD43B" alt="Vite">
  <img src="https://img.shields.io/badge/API-PokéAPI-blue?style=for-the-badge" alt="PokéAPI">
</div>

<div align="center">
  <h3>🌟 A modern and responsive web application to explore the Pokémon world</h3>
  
  [![Demo](https://img.shields.io/badge/Live_Demo-Visit-brightgreen?style=for-the-badge&logo=vercel)](https://your-demo-link.com)
  [![Version](https://img.shields.io/badge/Version-1.0.0-blue?style=for-the-badge)](https://github.com/your-username/pokedex)
</div>

---

## 📖 About

This project is a modern **Interactive Pokédex** built with Vue.js 3 and TypeScript. It allows users to search and explore Pokémon with an elegant and fully responsive interface.

### ✨ Features

- 🔍 **Real-time search** - Find your favorite Pokémon instantly
- 📱 **Responsive design** - Works perfectly on all devices
- 🎨 **Smooth animations** - Modern transitions and visual effects
- ⚡ **Optimized performance** - Fast loading and reactive interface
- 🌈 **Modern interface** - Clean design with Tailwind CSS
- 🔄 **Loading states** - Visual indicators for better UX

---

## 🚀 Technologies Used

<div align="center">

| Technology | Version | Description |
|-------------|---------|-------------|
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg" width="20" height="20"> **Vue.js** | 3.5.21 | Progressive JavaScript framework |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" width="20" height="20"> **TypeScript** | 5.8.3 | JavaScript with static typing |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" width="20" height="20"> **Tailwind CSS** | 4.1.13 | Utility-first CSS framework |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vitejs/vitejs-original.svg" width="20" height="20"> **Vite** | 7.1.7 | Ultra-fast build tool |
| 🌐 **PokéAPI** | - | Public API for Pokémon data |

</div>

---

## 🛠️ Installation and Setup

### Prerequisites

- **Node.js** (version 18 or higher)
- **npm** or **yarn**

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/pokedex.git
   cd pokedex
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run development server**
   ```bash
   npm run dev
   ```

4. **Open in browser**
   ```
   http://localhost:5173
   ```

### Available Scripts

```bash
# Development server
npm run dev

# Production build
npm run build

# Preview build
npm run preview
```

---

## 📱 Responsive Design

The application is fully responsive and adapts to all screen types:

| Screen Size | Columns | Device |
|----------------|----------|----------|
| < 475px | 1 | Smartphones |
| 475px - 640px | 2 | Large smartphones |
| 640px - 768px | 2 | Portrait tablets |
| 768px - 1024px | 3 | Landscape tablets |
| 1024px - 1280px | 4 | Laptops |
| 1280px - 1536px | 5 | Desktops |
| 1536px+ | 6 | Large screens |

---

## 🎯 Detailed Features

### 🔍 Search System
- Real-time search by Pokémon name
- Intuitive interface with French placeholder
- Instant results with transition animation

### 🎨 User Interface
- **Pokémon cards** with detailed information:
  - Pokémon image
  - Name
  - Health Points (HP)
  - Attack (ATK)
  - Defense (DEF)
- **Interactive hover effects** on all elements
- **Elegant loading animations**
- **Smooth transitions** between states

### 📊 Pokémon Data
- Uses PokéBuild API for up-to-date data
- Displays main statistics
- High-quality Pokémon images

---

## 🏗️ Project Architecture

```
src/
├── components/
│   ├── PokemonCard.vue      # Individual Pokémon card
│   ├── PokemonList.vue      # Responsive Pokémon list
│   └── PokemonSearch.vue    # Search component
├── App.vue                  # Main component
├── main.ts                  # Application entry point
└── style.css               # Global styles and Tailwind CSS
```

---

## 🎨 Customization

### Modify Colors
Colors can be customized in `tailwind.config.js`:

```javascript
theme: {
  extend: {
    colors: {
      'pokemon-blue': '#3B82F6',
      'pokemon-red': '#EF4444',
      'pokemon-yellow': '#F59E0B',
    }
  }
}
```

### Add New Features
- **Type filters**: Add filter buttons by Pokémon type
- **Pagination**: Implement pagination for better performance
- **Favorites**: Favorites system with local storage
- **Comparator**: Compare statistics of multiple Pokémon

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. **Fork** the project
2. **Create** a feature branch (`git checkout -b feature/AmazingFeature`)
3. **Commit** your changes (`git commit -m 'Add some AmazingFeature'`)
4. **Push** to the branch (`git push origin feature/AmazingFeature`)
5. **Open** a Pull Request

---

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

## 👨‍💻 Author

**Your Name**
- GitHub: [@your-username](https://github.com/your-username)
- LinkedIn: [Your Profile](https://linkedin.com/in/your-profile)

---

## 🙏 Acknowledgments

- [PokéAPI](https://pokebuildapi.fr/) for the free Pokémon data API
- [Vue.js](https://vuejs.org/) for the amazing framework
- [Tailwind CSS](https://tailwindcss.com/) for the design system
- [Vite](https://vitejs.dev/) for the ultra-fast build tool

---

<div align="center">
  <p>Made with ❤️ and Vue.js</p>
  <p>⭐ Feel free to give a star if this project helped you!</p>
</div>
