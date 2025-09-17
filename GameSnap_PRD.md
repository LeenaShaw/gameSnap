# Product Requirements Document (PRD) – GameSnap
**A Lightweight Client-Side Game Portal for Quick Mental Breaks**

---

## 1. Vision & Purpose Statement
GameSnap is a **zero-dependency, browser-only** game portal that delivers instant mental refreshment through bite-sized gaming experiences. Built for rapid prototyping and vibe coding, it prioritizes simplicity, speed, and immediate playability over complex features.

**Core Philosophy**: Click → Play → Refresh → Return to Work

## 2. Target Audience & Context
**Primary Users:**
- Developers taking 2-5 minute coding breaks
- Students between study sessions
- Office workers seeking quick mental resets

**Usage Context:**
- Quick breaks (30 seconds to 5 minutes)
- Desktop browsers (Chrome, Firefox, Edge)
- No installation or signup required
- Works offline after first load

## 3. Core Features (Prototype Scope)

### Tier 1: Essential MVP (30-40 minutes)
1. **Landing Portal** (`index.html`)
   - Clean grid layout with game thumbnails
   - Retro-inspired design (8-bit/pixel aesthetic)
   - Direct navigation to games

2. **2048 Mini** - Core sliding puzzle mechanics
3. **Memory Match** - Simple card flip memory game
4. **Word Scramble** - Unscramble 4-6 letter words

### Tier 2: Polish Features (15-20 minutes)
- Basic scoring display per game
- "Back to Portal" navigation
- Responsive design for different screen sizes

### Tier 3: Nice-to-Have (if time permits)
- Simple animations and transitions
- Local storage for high scores
- Sound toggle (on/off)

## 4. Key User Flows

### Primary Flow: Game Discovery & Play
```
Landing Page → Select Game → Play → View Score → Return to Portal
└─ 3 clicks maximum from start to gameplay
```

### Secondary Flow: Quick Replay
```
Game Over → "Play Again" → Instant Restart
└─ 1 click to replay same game
```

## 5. Technical Constraints (Vibe Coding Optimized)

### Must-Haves:
- **Pure client-side**: HTML + CSS + Vanilla JavaScript only
- **No build tools**: Direct file serving, no bundlers
- **No external dependencies**: No CDNs, libraries, or APIs
- **Single-file games**: Each game is self-contained
- **Fast iteration**: Changes visible with simple browser refresh

### File Structure:
```
/
├── index.html          (Portal/Landing page)
├── styles/
│   └── global.css      (Shared styles)
├── games/
│   ├── 2048.html
│   ├── memory.html
│   └── wordscramble.html
└── assets/
    └── sounds/ (optional)
```

## 6. Success Metrics (1-Hour Workshop)

### Functional Success:
- [ ] All 3 core games load and are playable
- [ ] Portal navigation works without errors
- [ ] Games complete successfully (win/lose states)
- [ ] Responsive on desktop browsers

### Time-Based Success:
- [ ] Basic MVP playable within 45 minutes
- [ ] Polish features added in remaining 15 minutes
- [ ] Zero game-breaking bugs

### User Experience Success:
- [ ] < 2 seconds from portal click to game start
- [ ] Intuitive controls (no instructions needed)
- [ ] Clear visual feedback for all interactions

## 7. Design Principles

### Vibe Coding Friendly:
1. **Start Simple**: Get one game working before adding features
2. **Copy-Paste Friendly**: Reusable code snippets between games
3. **Visual First**: Focus on what's immediately visible
4. **Progressive Enhancement**: Core functionality first, polish second

### User Experience:
1. **Instant Gratification**: Games start immediately
2. **Clear Feedback**: Obvious win/lose/score states
3. **Familiar Mechanics**: Use well-known game patterns
4. **Minimal Cognitive Load**: No complex rules or tutorials

## 8. Implementation Priority

### Phase 1 (First 20 minutes):
- Create basic HTML structure for portal
- Implement one complete game (Memory Match recommended)
- Basic CSS styling

### Phase 2 (Next 20 minutes):
- Add second game (2048 Mini)
- Improve portal styling and navigation
- Test cross-game navigation

### Phase 3 (Final 20 minutes):
- Add third game (Word Scramble)
- Polish UI/UX
- Add scoring and "play again" functionality
- Final testing and bug fixes

## 9. Risk Mitigation

### Time Management Risks:
- **Over-engineering**: Stick to vanilla JS, avoid complex patterns
- **Feature creep**: Complete Tier 1 before moving to Tier 2
- **Perfect pixel pushing**: Function over form initially

### Technical Risks:
- **Browser compatibility**: Test in Chrome first, then Firefox
- **Mobile responsiveness**: Desktop-first approach, mobile as stretch goal
- **Performance**: Keep games lightweight (< 100 lines JS each)

---

**Ready to Build**: This PRD is designed for immediate implementation. Start with the portal structure and one working game, then iterate rapidly.