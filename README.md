# 🎮 Pokédex Interactif

<div align="center">
  <img src="https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D" alt="Vue.js">
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/Vite-B73E9E?style=for-the-badge&logo=vite&logoColor=FFD43B" alt="Vite">
  <img src="https://img.shields.io/badge/API-PokéAPI-blue?style=for-the-badge" alt="PokéAPI">
</div>

<div align="center">
  <h3>🌟 Une application web moderne et responsive pour explorer le monde des Pokémon</h3>
  
  [![Demo](https://img.shields.io/badge/Live_Demo-Visiter-brightgreen?style=for-the-badge&logo=vercel)](https://your-demo-link.com)
  [![Version](https://img.shields.io/badge/Version-1.0.0-blue?style=for-the-badge)](https://github.com/your-username/pokedex)
</div>

---

## 📖 À Propos

Ce projet est une **Pokédex interactive** moderne construite avec Vue.js 3 et TypeScript. Elle permet aux utilisateurs de rechercher et d'explorer les Pokémon avec une interface utilisateur élégante et entièrement responsive.

### ✨ Fonctionnalités

- 🔍 **Recherche en temps réel** - Trouvez vos Pokémon préférés instantanément
- 📱 **Design responsive** - Fonctionne parfaitement sur tous les appareils
- 🎨 **Animations fluides** - Transitions et effets visuels modernes
- ⚡ **Performance optimisée** - Chargement rapide et interface réactive
- 🌈 **Interface moderne** - Design épuré avec Tailwind CSS
- 🔄 **États de chargement** - Indicateurs visuels pour une meilleure UX

---

## 🚀 Technologies Utilisées

<div align="center">

| Technologie | Version | Description |
|-------------|---------|-------------|
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg" width="20" height="20"> **Vue.js** | 3.5.21 | Framework JavaScript progressif |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" width="20" height="20"> **TypeScript** | 5.8.3 | JavaScript avec typage statique |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" width="20" height="20"> **Tailwind CSS** | 4.1.13 | Framework CSS utilitaire |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vitejs/vitejs-original.svg" width="20" height="20"> **Vite** | 7.1.7 | Outil de build ultra-rapide |
| 🌐 **PokéAPI** | - | API publique pour les données Pokémon |

</div>

---

## 🛠️ Installation et Configuration

### Prérequis

- **Node.js** (version 18 ou supérieure)
- **npm** ou **yarn**

### Installation

1. **Cloner le repository**
   ```bash
   git clone https://github.com/your-username/pokedex.git
   cd pokedex
   ```

2. **Installer les dépendances**
   ```bash
   npm install
   ```

3. **Lancer le serveur de développement**
   ```bash
   npm run dev
   ```

4. **Ouvrir dans le navigateur**
   ```
   http://localhost:5173
   ```

### Scripts Disponibles

```bash
# Serveur de développement
npm run dev

# Build de production
npm run build

# Prévisualisation du build
npm run preview
```

---

## 📱 Responsive Design

L'application est entièrement responsive et s'adapte à tous les types d'écrans :

| Taille d'écran | Colonnes | Appareil |
|----------------|----------|----------|
| < 475px | 1 | Smartphones |
| 475px - 640px | 2 | Grands smartphones |
| 640px - 768px | 2 | Tablettes portrait |
| 768px - 1024px | 3 | Tablettes paysage |
| 1024px - 1280px | 4 | Laptops |
| 1280px - 1536px | 5 | Desktops |
| 1536px+ | 6 | Grands écrans |

---

## 🎯 Fonctionnalités Détaillées

### 🔍 Système de Recherche
- Recherche en temps réel par nom de Pokémon
- Interface intuitive avec placeholder en français
- Résultats instantanés avec animation de transition

### 🎨 Interface Utilisateur
- **Cards Pokémon** avec informations détaillées :
  - Image du Pokémon
  - Nom
  - Points de Vie (PV)
  - Attaque (ATK)
  - Défense (DEF)
- **Effets hover** interactifs sur tous les éléments
- **Animations de chargement** élégantes
- **Transitions fluides** entre les états

### 📊 Données Pokémon
- Utilisation de l'API PokéBuild pour des données à jour
- Affichage des statistiques principales
- Images haute qualité des Pokémon

---

## 🏗️ Architecture du Projet

```
src/
├── components/
│   ├── PokemonCard.vue      # Carte individuelle de Pokémon
│   ├── PokemonList.vue      # Liste responsive des Pokémon
│   └── PokemonSearch.vue    # Composant de recherche
├── App.vue                  # Composant principal
├── main.ts                  # Point d'entrée de l'application
└── style.css               # Styles globaux et Tailwind CSS
```

---

## 🎨 Personnalisation

### Modifier les Couleurs
Les couleurs peuvent être personnalisées dans `tailwind.config.js` :

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

### Ajouter de Nouvelles Fonctionnalités
- **Filtres par type** : Ajouter des boutons de filtre par type de Pokémon
- **Pagination** : Implémenter une pagination pour de meilleures performances
- **Favoris** : Système de favoris avec stockage local
- **Comparateur** : Comparer les statistiques de plusieurs Pokémon

---

## 🤝 Contribution

Les contributions sont les bienvenues ! Pour contribuer :

1. **Fork** le projet
2. **Créer** une branche pour votre fonctionnalité (`git checkout -b feature/AmazingFeature`)
3. **Commit** vos changements (`git commit -m 'Add some AmazingFeature'`)
4. **Push** vers la branche (`git push origin feature/AmazingFeature`)
5. **Ouvrir** une Pull Request

---

## 📄 Licence

Ce projet est sous licence MIT. Voir le fichier `LICENSE` pour plus de détails.

---

## 👨‍💻 Auteur

**Votre Nom**
- GitHub: [@your-username](https://github.com/your-username)
- LinkedIn: [Votre Profil](https://linkedin.com/in/your-profile)

---

## 🙏 Remerciements

- [PokéAPI](https://pokebuildapi.fr/) pour l'API gratuite des données Pokémon
- [Vue.js](https://vuejs.org/) pour le framework incroyable
- [Tailwind CSS](https://tailwindcss.com/) pour le système de design
- [Vite](https://vitejs.dev/) pour l'outil de build ultra-rapide

---

<div align="center">
  <p>Fait avec ❤️ et Vue.js</p>
  <p>⭐ N'hésitez pas à donner une étoile si ce projet vous a aidé !</p>
</div>