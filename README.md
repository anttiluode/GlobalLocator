🌍 Global Locator: Day & Night Edition

Now live at: 

https://anttiluode.github.io/GlobalLocator/

A modern, interactive geography guessing game built with pure HTML, CSS, and JavaScript. Test your knowledge of world geography by locating countries, US states, and major cities on an interactive map!
Show Image Show Image Show Image Show Image
✨ Features
🎮 Game Modes

World Countries - Guess the location of any country worldwide
US States - Focus on United States geography with close-up view
Major Cities - Locate major world cities (100k+ population)
European Countries - Challenge yourself with European geography
Asian Countries - Test your knowledge of Asian nations

🎯 Difficulty Levels

Easy - 45 seconds per round, 0.8x score multiplier
Medium - 30 seconds per round, 1.0x score multiplier
Hard - 15 seconds per round, 1.5x score multiplier

🌅 Visual Themes

Night Mode - Dark theme with neon accents and atmospheric lighting
Day Mode - Clean, bright theme perfect for daytime play
Smart map tiles that automatically switch with your theme
Glass morphism UI with modern blur effects

🎵 Audio Experience

Ambient soundscape that loops continuously for immersion
Audio feedback with different tones for accuracy levels
Mute/unmute toggle with preference saving
Browser-friendly audio that respects autoplay policies

📊 Scoring System

Dynamic scoring based on distance accuracy
Streak tracking for consecutive good guesses
High score persistence saved locally per mode/difficulty
Floating score animations for immediate feedback
Skip option available (-500 points penalty)

🚀 Quick Start
Option 1: Direct Download

Save the HTML file to your computer
Open it in any modern web browser
Start playing immediately!

Option 2: GitHub Pages Deployment

Try it at: 

https://anttiluode.github.io/GlobalLocator/

Option 3: Local Development
bash# Clone the repository
git clone https://github.com/anttiluode/GlobaLocator.git

# Navigate to the directory
cd global-locator-game

# Serve locally (optional, can also just open the HTML file)
python -m http.server 8000
# or
npx serve .
🎮 How to Play

Choose your game mode from the dropdown menu
Select difficulty level (Easy/Medium/Hard)
Toggle day/night mode to your preference
Enable audio for the full experience
Read the target location displayed at the top
Click on the map where you think the location is
See your results with distance, score, and accuracy
Continue to next round or skip if stuck
Beat your high score and build winning streaks!

🛠️ Technical Details
Built With

Leaflet.js - Interactive map rendering
Pure HTML/CSS/JavaScript - No build process required
REST Countries API - Live country data loading
Local Storage - High score and preference persistence
Web Audio API - Sound effects and ambient audio

Browser Compatibility

✅ Chrome 80+
✅ Firefox 75+
✅ Safari 13+
✅ Edge 80+
📱 Mobile browsers supported

Data Sources

Countries: REST Countries API via GitHub
US States: Hardcoded reliable coordinates
World Cities: Curated list of major metropolitan areas
Map Tiles: CartoDB (Dark/Light themes)

🎨 Customization
Themes
The game automatically adapts to your theme preference:
css/* Dark theme variables */
--dark-bg: #1a1a2e;
--dark-accent: #00f5ff;

/* Light theme variables */
--light-bg: #f0f2f5;
--light-accent: #3498db;
Game Settings
Modify the configuration object to adjust gameplay:
javascriptconst CONFIG = {
    STARTING_SCORE: 5000,
    MAX_SCORE_PER_ROUND: 2500,
    SKIP_PENALTY: 500,
    DIFFICULTY_SETTINGS: {
        easy: { time: 45, multiplier: 0.8 },
        medium: { time: 30, multiplier: 1.0 },
        hard: { time: 15, multiplier: 1.5 }
    }
};
Adding New Locations
To add custom location sets, extend the gameData object:
javascriptgameData.customLocations = [
    {name: "Location Name", coords: [latitude, longitude]},
    // Add more locations...
];
📱 Mobile Experience
The game is fully responsive and optimized for mobile devices:

Touch-friendly interface with larger tap targets
Responsive design that adapts to screen size
Optimized fonts and UI scaling
Gesture support for map interaction

🔧 Troubleshooting
Audio Not Playing

Ensure you've clicked somewhere on the page first (browser autoplay policy)
Check that audio is enabled with the 🔊 button
Verify your browser supports Web Audio API

Map Not Loading

Check your internet connection for tile loading
Ensure JavaScript is enabled in your browser
Try refreshing the page if tiles appear broken

Country Data Not Loading

The game includes fallback data for offline use
Check browser console for any network errors
Verify the REST Countries API is accessible

📄 License
This project is open source and available under the MIT License.
