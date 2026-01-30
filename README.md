# TimeCops

A simple, elegant stopwatch app for tracking multiple timers simultaneously. Perfect for time management, productivity tracking, workouts, cooking, and any scenario where you need to track multiple timers at once.

![TimeCops](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

**[🚀 Try it live!](https://sri.github.io/timecops/timecops.html)**

## Features

- **Multiple Stopwatches** - Track as many timers as you need simultaneously
- **Custom Names** - Click any label to give your stopwatch a meaningful name
- **Easy Controls** - Simple click to start/stop timing
- **Precise Timing** - Millisecond accuracy (MM:SS:mmm format)
- **5 Beautiful Themes** - Choose from Default, Matrix, Business, Sports, or Kids themes
- **URL Templates** - Your configuration and theme are saved in the URL for easy bookmarking and sharing
- **Beautiful Design** - Clean, modern interface with smooth animations
- **Fully Responsive** - Works perfectly on desktop, tablet, and mobile devices
- **No Installation** - Just open the HTML file in any browser

## Quick Start

1. Download or clone this repository
2. Open `timecops.html` in your web browser
3. Start timing!

```bash
# Clone the repository
git clone https://github.com/yourusername/timecops.git

# Open in browser
open timecops.html
```

## How to Use

### Basic Operations

- **Start/Stop Timer**: Click on the stopwatch circle to toggle timing
- **Name a Stopwatch**: Click on the label text below the time display to edit the name
  - Press `Enter` or click away to save
  - Press `Escape` to cancel
- **Add Stopwatch**: Click the "+ Add Stopwatch" button at the bottom
- **Delete Stopwatch**: Hover over a stopwatch and click the × button in the top-right corner
- **Change Theme**: Use the theme selector dropdown in the header to switch between visual themes

### Themes

TimeCops includes 5 distinct themes to match your mood or use case:

1. **Default** - Purple gradient with clean, modern design
2. **Matrix** 🟢 - Iconic black and green hacker aesthetic with glowing effects and monospace fonts
3. **Business** 💼 - Professional slate gray with corporate blue accents, perfect for work environments
4. **Sports** 🏆 - Bold and energetic with red/yellow colors, uppercase fonts, and stadium-style vibes
5. **Kids** 🎨 - Bright, joyful multi-color gradient with bouncing animations and playful design

Themes are automatically saved in both localStorage and the URL, so your bookmarked templates preserve the visual style.

### URL Templates

TimeCops automatically saves your stopwatch configuration and theme in the URL, making it easy to create reusable templates:

1. Set up your stopwatches with custom names and choose a theme
2. The URL updates automatically (e.g., `timecops.html#theme=matrix&timeclocks=Work&Break&Exercise`)
3. Bookmark the URL to save your template
4. Share the URL with others or use it across devices

**URL Format:**
- With theme and stopwatches: `#theme=matrix&timeclocks=Work&Break`
- Just stopwatches (default theme): `#timeclocks=Work&Break`
- Just theme: `#theme=sports`

**Note**: The URL stays clean on initial load. It only updates once you interact with the app (naming, adding, deleting stopwatches, or changing themes).

### Template Examples

Create different setups for different workflows:

#### Pomodoro Technique (Business Theme)
```
timecops.html#theme=business&timeclocks=Work&Short%20Break&Long%20Break
```
Set up timers for focused work sessions and breaks with a professional look.

#### Workout Intervals (Sports Theme)
```
timecops.html#theme=sports&timeclocks=Warmup&Exercise%201&Exercise%202&Rest&Cooldown
```
Track different exercises and rest periods with an energetic sports aesthetic.

#### Coding Sprint (Matrix Theme)
```
timecops.html#theme=matrix&timeclocks=Hack&Debug&Deploy&Review
```
Perfect for development sessions with that iconic hacker vibe.

#### Kids Activities (Kids Theme)
```
timecops.html#theme=kids&timeclocks=Playtime&Snack&Storytime&Nap
```
Track children's activities with bright, fun colors and playful animations.

#### Cooking Multiple Dishes
```
timecops.html#timeclocks=Main%20Dish&Side%20Dish&Dessert
```
Time multiple cooking tasks simultaneously (default theme).

#### Team Meetings (Business Theme)
```
timecops.html#theme=business&timeclocks=Speaker%201&Speaker%202&Q%26A&Wrap%20Up
```
Track time allocation for different agenda items in a professional setting.

## Use Cases

- **Productivity**: Pomodoro technique, time blocking, task tracking
- **Fitness**: Interval training, circuit workouts, rest periods
- **Cooking**: Multi-dish preparation, precise timing for recipes
- **Meetings**: Speaker time, agenda items, break scheduling
- **Education**: Test timing, activity duration, classroom management
- **Gaming**: Speed runs, challenge timing, turn timers
- **Creative Work**: Time-boxing tasks, practice sessions, breaks

## Technical Details

- **No Dependencies**: Pure HTML, CSS, and vanilla JavaScript
- **No Backend**: Everything runs client-side in the browser
- **Privacy-First**: No data collection, no analytics, no cookies (only localStorage for theme preference)
- **Offline Capable**: Works without an internet connection
- **Lightweight**: Single HTML file (~15KB with all themes)
- **CSS Variables**: Theme system uses CSS custom properties for easy customization
- **localStorage**: Only used to remember your last selected theme

## Browser Compatibility

TimeCops works in all modern browsers:
- Chrome/Edge (latest)
- Firefox (latest)
- Safari (latest)
- Mobile browsers (iOS Safari, Chrome Mobile)

## Development

The entire application is contained in a single HTML file (`timecops.html`) with embedded CSS and JavaScript. To modify:

1. Open `timecops.html` in your favorite text editor
2. Make your changes
3. Refresh in browser to test

### Structure

- **HTML**: Semantic markup with modal overlay for the about section
- **CSS**: Flexbox and Grid layout with responsive design
- **JavaScript**: ES6+ class-based stopwatch implementation with URL state management

## Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests
- Improve documentation

## License

MIT License - feel free to use this project for personal or commercial purposes.

## Acknowledgments

Built with [Claude Code](https://claude.com/claude-code) using the Claude Sonnet 4.5 model.

Made with ❤️ for everyone who needs to track time efficiently.

---

**Note**: This is a client-side application. Your stopwatch configurations are stored only in the URL (which you can bookmark). No data is sent to any server.
