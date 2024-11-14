# 🎵 Audio Visualizer

A sleek, responsive audio visualization tool built with vanilla JavaScript and the Web Audio API. Transform your audio files into dynamic, real-time visual representations with this easy-to-use web application.

## ✨ Features

- 🎨 Real-time frequency visualization
- 🎚️ Volume control
- 📱 Responsive design that works on all devices
- 🎯 Support for various audio file formats



## 🛠️ Technology Stack

- HTML5
- CSS3
- JavaScript (ES6+)
- Web Audio API
- Canvas API

## 📖 How It Works

The visualizer uses the Web Audio API to analyze audio frequencies in real-time. Here's the technical flow:

1. Audio file is loaded and decoded using `AudioContext`
2. Sound data is processed through an analyzer node
3. Frequency data is extracted using `getByteFrequencyData`
4. Canvas API renders the visualization with dynamic bars
5. RequestAnimationFrame creates smooth animations

## 🎯 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Local development server (optional)

### Installation

1. Clone the repository:
```bash
git clone https://github.com/ByteOfWaffle/audio-visualizer.git
```

2. Navigate to the project directory:
```bash
cd audio-visualizer
```

3. Open `index.html` in your browser or serve it through a local development server.

### Usage

1. Click "Choose Audio File" to select your audio file
2. Press the "Play" button to start visualization
3. Use the volume slider to adjust audio level
4. Watch as your audio comes to life!

## 🎨 Customization

You can customize the visualizer by modifying these parameters in the code:

```javascript
// In the initAudio() function:
analyser.fftSize = 256; // Adjust for more/fewer frequency bars
analyser.smoothingTimeConstant = 0.8; // Adjust for smoother/sharper transitions

// In the startVisualization() function:
const gradient = ctx.createLinearGradient(0, canvas.height, 0, canvas.height - barHeight);
gradient.addColorStop(0, '#4a90e2'); // Change colors here
gradient.addColorStop(1, '#357abd'); // And here
```

## 📱 Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)


## 📄 License

This project is licensed under the MIT License

## 🙏 Acknowledgments

- Inspired by various audio visualization projects
- Thanks to the Web Audio API team for the amazing documentation