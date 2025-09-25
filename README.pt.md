# 🎮 Pokédex Interativo

<div align="center">
  <img src="https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vue.js&logoColor=4FC08D" alt="Vue.js">
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript">
  <img src="https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind CSS">
  <img src="https://img.shields.io/badge/Vite-B73E9E?style=for-the-badge&logo=vite&logoColor=FFD43B" alt="Vite">
  <img src="https://img.shields.io/badge/API-PokéAPI-blue?style=for-the-badge" alt="PokéAPI">
</div>

<div align="center">
  <h3>🌟 Uma aplicação web moderna e responsiva para explorar o mundo dos Pokémon</h3>
  
  [![Demo](https://img.shields.io/badge/Demo_Ao_Vivo-Visitar-brightgreen?style=for-the-badge&logo=vercel)](https://your-demo-link.com)
  [![Versão](https://img.shields.io/badge/Versão-1.0.0-blue?style=for-the-badge)](https://github.com/your-username/pokedex)
</div>

---

## 📖 Sobre o Projeto

Este projeto é uma **Pokédex interativa** moderna construída com Vue.js 3 e TypeScript. Permite aos usuários pesquisar e explorar Pokémon com uma interface elegante e totalmente responsiva.

### ✨ Funcionalidades

- 🔍 **Pesquisa em tempo real** - Encontre seus Pokémon favoritos instantaneamente
- 📱 **Design responsivo** - Funciona perfeitamente em todos os dispositivos
- 🎨 **Animações fluidas** - Transições e efeitos visuais modernos
- ⚡ **Performance otimizada** - Carregamento rápido e interface reativa
- 🌈 **Interface moderna** - Design limpo com Tailwind CSS
- 🔄 **Estados de carregamento** - Indicadores visuais para melhor UX

---

## 🚀 Tecnologias Utilizadas

<div align="center">

| Tecnologia | Versão | Descrição |
|-------------|---------|-------------|
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vuejs/vuejs-original.svg" width="20" height="20"> **Vue.js** | 3.5.21 | Framework JavaScript progressivo |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/typescript/typescript-original.svg" width="20" height="20"> **TypeScript** | 5.8.3 | JavaScript com tipagem estática |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/tailwindcss/tailwindcss-original.svg" width="20" height="20"> **Tailwind CSS** | 4.1.13 | Framework CSS utilitário |
| <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/vitejs/vitejs-original.svg" width="20" height="20"> **Vite** | 7.1.7 | Ferramenta de build ultra-rápida |
| 🌐 **PokéAPI** | - | API pública para dados dos Pokémon |

</div>

---

## 🛠️ Instalação e Configuração

### Pré-requisitos

- **Node.js** (versão 18 ou superior)
- **npm** ou **yarn**

### Instalação

1. **Clonar o repositório**
   ```bash
   git clone https://github.com/your-username/pokedex.git
   cd pokedex
   ```

2. **Instalar as dependências**
   ```bash
   npm install
   ```

3. **Executar o servidor de desenvolvimento**
   ```bash
   npm run dev
   ```

4. **Abrir no navegador**
   ```
   http://localhost:5173
   ```

### Scripts Disponíveis

```bash
# Servidor de desenvolvimento
npm run dev

# Build de produção
npm run build

# Pré-visualização do build
npm run preview
```

---

## 📱 Design Responsivo

A aplicação é totalmente responsiva e se adapta a todos os tipos de tela:

| Tamanho da Tela | Colunas | Dispositivo |
|----------------|----------|----------|
| < 475px | 1 | Smartphones |
| 475px - 640px | 2 | Smartphones grandes |
| 640px - 768px | 2 | Tablets retrato |
| 768px - 1024px | 3 | Tablets paisagem |
| 1024px - 1280px | 4 | Laptops |
| 1280px - 1536px | 5 | Desktops |
| 1536px+ | 6 | Telas grandes |

---

## 🎯 Funcionalidades Detalhadas

### 🔍 Sistema de Pesquisa
- Pesquisa em tempo real por nome do Pokémon
- Interface intuitiva com placeholder em francês
- Resultados instantâneos com animação de transição

### 🎨 Interface do Usuário
- **Cards Pokémon** com informações detalhadas :
  - Imagem do Pokémon
  - Nome
  - Pontos de Vida (PV)
  - Ataque (ATK)
  - Defesa (DEF)
- **Efeitos hover** interativos em todos os elementos
- **Animações de carregamento** elegantes
- **Transições fluidas** entre os estados

### 📊 Dados dos Pokémon
- Uso da API PokéBuild para dados atualizados
- Exibição das estatísticas principais
- Imagens de alta qualidade dos Pokémon

---

## 🏗️ Arquitetura do Projeto

```
src/
├── components/
│   ├── PokemonCard.vue      # Card individual do Pokémon
│   ├── PokemonList.vue      # Lista responsiva dos Pokémon
│   └── PokemonSearch.vue    # Componente de pesquisa
├── App.vue                  # Componente principal
├── main.ts                  # Ponto de entrada da aplicação
└── style.css               # Estilos globais e Tailwind CSS
```

---

## 🎨 Personalização

### Modificar as Cores
As cores podem ser personalizadas em `tailwind.config.js` :

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

### Adicionar Novas Funcionalidades
- **Filtros por tipo** : Adicionar botões de filtro por tipo de Pokémon
- **Paginação** : Implementar paginação para melhor performance
- **Favoritos** : Sistema de favoritos com armazenamento local
- **Comparador** : Comparar estatísticas de vários Pokémon

---

## 🤝 Contribuição

Contribuições são bem-vindas! Para contribuir:

1. **Fork** o projeto
2. **Criar** uma branch para sua funcionalidade (`git checkout -b feature/AmazingFeature`)
3. **Commit** suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. **Push** para a branch (`git push origin feature/AmazingFeature`)
5. **Abrir** uma Pull Request

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

---

## 👨‍💻 Autor

**Seu Nome**
- GitHub: [@your-username](https://github.com/your-username)
- LinkedIn: [Seu Perfil](https://linkedin.com/in/your-profile)

---

## 🙏 Agradecimentos

- [PokéAPI](https://pokebuildapi.fr/) pela API gratuita dos dados dos Pokémon
- [Vue.js](https://vuejs.org/) pelo framework incrível
- [Tailwind CSS](https://tailwindcss.com/) pelo sistema de design
- [Vite](https://vitejs.dev/) pela ferramenta de build ultra-rápida

---

<div align="center">
  <p>Feito com ❤️ e Vue.js</p>
  <p>⭐ Não hesite em dar uma estrela se este projeto te ajudou!</p>
</div>
