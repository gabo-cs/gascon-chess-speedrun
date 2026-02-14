# Gascón Chess Speedrun Library

Complete library of GM Gascón's Chess games from the "Cómo Piensa un GM" speedrun series.

## 🎯 About

This project catalogs all games from GM Gascón's popular YouTube speedrun series, making it easy to find and study specific openings, positions, and games by rating range.

**Features:**
- 🔍 Search and filter games by opening, variation, and opponent rating
- 📺 Direct links to exact YouTube timestamps for each game
- ♟️ Links to full game replays on Chess.com
- 🌓 Dark mode support
- 📱 Fully responsive design

## 🚀 Project Structure
```text
/
├── public/
├── src/
│   ├── components/
│   │   ├── GameCard.astro
│   │   └── Navbar.astro
│   ├── layouts/
│   │   └── Layout.astro
│   ├── pages/
│   │   ├── index.astro
│   │   ├── acerca-de.astro
│   │   └── game/
│   │       └── [slug].astro
│   ├── data/
│   │   └── games.json
│   └── styles/
│       └── global.css
└── package.json
```

## 🛠️ Tech Stack

- **[Astro](https://astro.build)** - Web framework
- **[Tailwind CSS](https://tailwindcss.com)** - Styling
- **TypeScript** - Type safety

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |
| `npm run astro -- --help` | Get help using the Astro CLI                     |

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

### Adding New Games

1. Fork the repository
2. Add game data to `src/data/games.json` following this format:
```json
{
  "slug": "unique-game-identifier",
  "opening_es": "Apertura",
  "opening_en": "Opening",
  "variation_es": "Variante (opcional)",
  "variation_en": "Variation (optional)",
  "white": "Player White",
  "black": "Player Black",
  "opponent_rating": 1500,
  "youtube_link": "https://youtube.com/watch?v=...",
  "chesscom_link": "https://chess.com/game/..."
}
```

**Note:** Please include both Spanish (`_es`) and English (`_en`) fields for openings and variations. We're planning to add i18n support in the future, so keeping everything translatable helps!

3. Create a pull request

### Other Contributions

- 🐛 Report bugs by opening an issue
- 💡 Suggest new features or improvements
- 📝 Improve documentation
- 🎨 Enhance UI/UX
- 🌍 Help with internationalization

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Credits

This project was created with the approval and encouragement of **GM Gascón** himself. He has green-lit the project and encouraged sharing it with the chess community.

- **GM Gascón** - For the incredible "Cómo Piensa un GM" speedrun series
- YouTube Channel: [@GasconChess](https://www.youtube.com/@GasconChess)

## 👀 Want to learn more about Astro?

Check out [Astro documentation](https://docs.astro.build) or jump into the [Astro Discord server](https://astro.build/chat).
