# Gorillas Game
A modern recreation of the classic QBasic Gorillas game using HTML5 Canvas and P5.js.

## Description
This is a turn-based artillery game where players control gorillas atop buildings, attempting to hit each other with exploding bananas. The game features dynamic city landscapes, wind effects, and physics-based projectile motion.

## Features
- Dynamic city generation with random building heights and window patterns
- Physics-based projectile motion affected by gravity and wind
- Two-player gameplay (Player vs AI)
- Persistent explosion holes in buildings
- Responsive design that scales with window size
- Score tracking system
- Simple AI opponent

## How to Play
1. **Setup**: The game automatically generates a cityscape with two gorillas positioned on buildings.
2. **Controls**:
   - **Angle** (0-360 degrees): Direction of the throw
   - **Velocity** (1-100): Power of the throw
3. **Gameplay**:
   - Players take turns throwing bananas
   - Wind affects banana trajectory (shown by red arrow at bottom)
   - Direct hits on opponent score a point
   - First player to score 3 points wins

## Technical Details

### Classes
- `Building`: Manages building properties and window generation
- `Gorilla`: Handles gorilla rendering and positioning
- `Banana`: Controls projectile physics and collision detection
- `Explosion`: Manages explosion animations and creates holes

### Key Functions
- `generateLevel()`: Creates new city layout
- `calculateAIShot()`: Determines AI player moves
- `windowResized()`: Handles responsive scaling
- `submitTurn()`: Processes player input
- `draw()`: Main game loop and rendering

## Technologies Used
- HTML5
- CSS3
- JavaScript
- P5.js library

## Setup
1. Clone the repository
2. Open `index.html` in a modern web browser
3. No additional installation required

## Dependencies
- P5.js (loaded via CDN)

## Browser Compatibility
- Chrome (recommended)
- Firefox
- Safari
- Edge

## Known Issues
- Extreme window resizing might affect gameplay physics
- AI difficulty is currently fixed

## Future Improvements
- Multiple AI difficulty levels
- Mobile touch controls
- Sound effects
- Multiplayer support
- Additional weapon types
- Save game progress
