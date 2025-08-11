# Ballad of the Balloons 🎈

An interactive audio-visual experience that transforms weather balloon data into music using granular synthesis and p5.js visualization.

## About

This project fetches real-time weather balloon data from the Sondehub API and creates an immersive experience where each balloon's atmospheric measurements influence the parameters of granular synthesis. The result is a unique "song" that represents the atmospheric conditions around the world.

## Features

- **Real-time data**: Fetches live weather balloon data from Sondehub API
- **Granular synthesis**: Each balloon creates audio grains based on its atmospheric data
- **Interactive visualization**: p5.js canvas showing balloon positions and data
- **Time control**: Slider to explore data across different time periods
- **Audio controls**: Play/pause, loop, and speed adjustment
- **Responsive design**: Works on desktop and mobile devices

## Technologies Used

- **p5.js** - Creative coding and visualization
- **Web Audio API** - Granular synthesis engine
- **Sondehub API** - Weather balloon data source
- **Vanilla JavaScript** - No frameworks, pure web technologies

## Getting Started

### Prerequisites

- Node.js (v16 or higher)
- Modern web browser with Web Audio API support

### Installation

1. Clone the repository:
   ```bash
   git clone <your-repo-url>
   cd balladOfTheBalloons
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```

4. Open your browser to `http://localhost:3000`

### Available Scripts

- `npm run dev` - Start development server
- `npm start` - Start development server (alias)
- `npm run build` - Build for production (no build step needed for static site)
- `npm run deploy` - Deploy to Vercel (requires Vercel CLI)

## How It Works

1. **Data Fetching**: The app fetches weather balloon data every 30 minutes from the Sondehub API
2. **Data Processing**: Each balloon's position, altitude, and atmospheric data is processed
3. **Audio Generation**: Granular synthesis creates audio grains based on balloon parameters
4. **Visualization**: p5.js renders the balloons on a world map with real-time updates
5. **User Interaction**: Users can control playback, explore different time periods, and adjust audio parameters

## Data Sources

- **Weather Balloon Data**: [Sondehub API](https://sondehub.org/)
- **Granular Synthesis Engine**: Based on work by [Michael Phipps](https://codepen.io/michaelphipps/pen/RBwbvv)
- **Audio Sample**: "Up Up and Away" by the 5th Dimension

## Project Structure

```
balladOfTheBalloons/
├── index.html              # Main HTML file
├── style.css               # Main stylesheet
├── sketchGrain.js          # Main JavaScript application
├── package.json            # Node.js dependencies and scripts
├── README.md               # Project documentation
├── .gitignore              # Git ignore rules
└── public/                 # Assets folder
    ├── upupandaway.mp3     # Audio sample
    ├── IRx500_01A.wav      # Reverb impulse response
    ├── View_of_Earth_from_a_stratospheric_sonde_2.jpg  # Background image
    └── radiosondeDataPreview.json  # Sample weather balloon data
```

## Development

This is a static website with no build process required. Simply edit the HTML, CSS, or JavaScript files and refresh your browser to see changes.

## Deployment

The project can be deployed to any static hosting service:

- **Vercel**: `npm run deploy` (recommended)
- **Netlify**: Drag and drop the project folder
- **GitHub Pages**: Push to a GitHub repository
- **Any static host**: Upload the files directly

## License

MIT License - see LICENSE file for details

## Credits

Created by Jasper Hall with assistance from Claude 3.5 Sonnet, ChatGPT-4o, and o1.
