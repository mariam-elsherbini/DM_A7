# React Tetris Enhancement Project

## Project Overview

This repository is a fork of [Chvin's React Tetris](https://github.com/chvin/react-tetris), enhanced as part of an assignment to demonstrate the capabilities of Aider, an AI-powered coding assistant. The original project is a classic Tetris game built using React and Redux, featuring responsive design that works across desktop and mobile devices.


## Original Project Functionality

The original React Tetris project features:

- Classic Tetris gameplay with React and Redux architecture
- Responsive design that works on both desktop and mobile devices
- Game controls via keyboard (desktop) or touch gestures (mobile)
- Pause functionality and score tracking
- Clean, retro-styled UI inspired by the Game Boy version of Tetris
- Sound effects and background music
- Game state persistence using localStorage

## Added Features

### 1. Power-Up System

I've implemented a power-up system that adds an extra strategic layer to the gameplay:

- **Power-up blocks**: Special blocks appear randomly on the board (identifiable by a star icon)
- **Types of power-ups**:
  - **Line Clear**: Instantly clears a random line on the board
  - **Slow Down**: Temporarily slows block descent speed for 10 seconds
  - **Score Boost**: Multiplies points gained for the next line clear by 3x

Power-ups are activated upon clearing a line containing a power-up block, adding strategic depth to the game.

### 2. Advanced Statistics Dashboard

A comprehensive statistics tracking system has been added:

- **Real-time metrics**: 
  - Average blocks per minute
  - Longest survival time
  - Power-up usage efficiency
  - Block distribution by type
- **Persistent statistics**: Game stats are saved between sessions
- **Shareable results**: Option to share high scores on social media
- **Visual data representation**: Charts showing performance over time

### 3. Customizable Themes

Added theme customization to personalize the gaming experience:

- **Multiple color schemes**: Classic, Dark Mode, Neon, Pastel
- **Custom block designs**: Alternative block patterns and styling
- **Background options**: Different grid patterns and background images
- **User preferences**: Theme settings are saved between sessions

## Implementation Process

The implementation process involved several stages:

1. **Understanding the codebase**: Using Aider to explore and understand the game's architecture
2. **Planning the features**: Breaking down complex additions into manageable components
3. **Implementation with Aider**: Using AI pair programming to write and refine code
4. **Testing and debugging**: Identifying and fixing issues in the implementation
5. **Documentation**: Creating comprehensive documentation of the new features

## Installation and Setup

```bash
# Clone the repository
git clone https://github.com/yourusername/react-tetris.git
cd react-tetris

# Install dependencies
npm install

# Start the development server
npm start
```

The game will be available at `http://localhost:3000`.

## Usage

### Desktop Controls:
- **Arrow Up**: Rotate block
- **Arrow Down**: Move block down
- **Arrow Left/Right**: Move block horizontally
- **Space**: Hard drop
- **P**: Pause game
- **S**: Sound on/off
- **R**: Reset game
- **T**: Toggle theme

### Mobile Controls:
- **Tap upper area**: Rotate block
- **Tap left/right area**: Move block horizontally
- **Tap bottom area**: Move block down
- **Menu buttons**: Access other functions

## Challenges and Solutions

### Challenge 1: Integrating Power-Ups into Game Logic
The existing game state management was complex, making it difficult to add new features without breaking existing functionality.

**Solution**: Used Aider to analyze the Redux state architecture and created a non-intrusive power-up system that extends rather than modifies the core game mechanics.

### Challenge 2: Performance Issues with Statistics Dashboard
Initial implementation of the statistics dashboard caused performance degradation during gameplay.

**Solution**: Implemented a more efficient data collection method and moved heavy calculations to happen only during game pauses or when the dashboard is actually visible.

### Challenge 3: Theme System Compatibility
Making the theme system work across all components required extensive CSS changes.

**Solution**: Used Aider to create a theme context provider and systematically updated the styling approach to use CSS variables, allowing for dynamic theme switching without performance impact.

## Credits

- Original project by [Chvin](https://github.com/chvin)
- Enhancements by [Your Name]
- Implemented with assistance from Aider

## License

[MIT License](LICENSE)
