# GameSnap 🎮

A lightweight, client-side game portal offering quick, casual games for mental refreshment during breaks. Built with pure HTML, CSS, and JavaScript - no dependencies required!

## 🎯 Features

- **Memory Match**: Test your memory with this classic card matching game
- **2048 Mini**: Slide numbered tiles to reach the coveted 2048 tile
- **Word Scramble**: Unscramble letters to form words with hints and categories

## 🚀 Quick Start

1. **Clone or download** this repository
2. **Open `index.html`** in any modern web browser
3. **Start playing** - no installation required!

### Alternative: Local Server
For the best experience, serve the files through a local HTTP server:

```bash
# Using Python (if installed)
python -m http.server 8000

# Using Node.js
npx serve -s . -p 8000

# Then visit http://localhost:8000
```

## 🎮 Games Overview

### Memory Match 🧠
- Flip cards to find matching pairs
- Score based on speed and accuracy
- Progressive difficulty with time tracking

### 2048 Mini 🔢
- Use arrow keys or WASD to move tiles
- Combine matching numbers to reach 2048
- Undo functionality and local high score tracking

### Word Scramble 📝
- 60-second time limit
- Category hints available
- Streak bonuses and skip functionality

## 📱 Browser Compatibility

- ✅ Chrome/Edge (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Mobile browsers (responsive design)

## 🛠️ Technical Details

- **Pure client-side**: No server required
- **Zero dependencies**: No external libraries
- **Lightweight**: < 100KB total
- **Responsive**: Works on desktop and mobile
- **Offline capable**: Runs locally after download

## 📁 Project Structure

```
/
├── index.html          # Main portal/landing page
├── styles/
│   └── global.css      # Shared styling with retro theme
├── games/
│   ├── memory.html     # Memory matching game
│   ├── 2048.html       # 2048 sliding puzzle
│   └── wordscramble.html # Word unscrambling game
└── README.md           # This file
```

## 🎨 Design Philosophy

- **Instant gratification**: Games start immediately
- **Retro aesthetic**: 8-bit inspired design with modern touches
- **Clear feedback**: Obvious win/lose/score states
- **Minimal cognitive load**: No complex rules or tutorials needed

## 🔧 Customization

### Adding New Words (Word Scramble)
Edit the `words` array in `games/wordscramble.html`:

```javascript
{word: 'EXAMPLE', hint: 'A demonstration or instance', category: 'EDUCATION'}
```

### Modifying Game Settings
- **Memory Match**: Change grid size by modifying the CSS grid and card generation logic
- **2048**: Adjust grid size or winning tile in the game class
- **Word Scramble**: Modify timer duration, scoring, or word categories

## 🏆 High Scores

- Memory Match: Stored per session
- 2048: Saved to local storage (persistent)
- Word Scramble: Session-based leaderboard

## 📝 License

Open source - feel free to modify and share!

---

**Built for quick mental breaks • No signup required • Play instantly**