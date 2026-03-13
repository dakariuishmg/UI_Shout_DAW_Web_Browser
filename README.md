# UI_Shout_DAW_Web_Browser
A professional-grade browser-based DAW (Digital Audio Workstation) with multi-track recording, MIDI piano roll, step sequencer, mixer, effects, and real-time audio processing.

Language: HTML
Dependencies: Web Audio API, Canvas API, Vanilla JavaScript, CSS Grid/Flexbox, LocalStorage API, Web MIDI API, MediaRecorder API
Topics: daw, audio-workstation, music-production, midi-sequencer, audio-recording, web-audio, synthesizer, audio-effects

# ui-shout

A professional-grade browser-based DAW (Digital Audio Workstation) with multi-track recording, MIDI piano roll, step sequencer, mixer, effects, and real-time audio processing.

## Features

- **Multi-track Recording**: Record and edit multiple audio tracks simultaneously
- **MIDI Piano Roll**: Create and edit MIDI sequences with an intuitive piano roll interface
- **Step Sequencer**: Program beats and patterns with a grid-based step sequencer
- **Professional Mixer**: Multi-channel mixer with volume, pan, and routing controls
- **Audio Effects**: Built-in effects including reverb, delay, compression, EQ, and distortion
- **Real-time Processing**: Low-latency audio processing using the Web Audio API
- **Synthesizers**: Built-in software synthesizers for sound generation
- **MIDI Support**: Connect external MIDI controllers via Web MIDI API
- **Project Management**: Save and load projects using LocalStorage
- **Export Audio**: Render and export your projects as audio files

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/ui-shout.git
cd ui-shout
```

2. Open `index.html` in a modern web browser:
```bash
# Using Python 3
python -m http.server 8000

# Using Node.js
npx serve

# Or simply open the file
open index.html
```

3. Navigate to `http://localhost:8000` in your browser

## Usage

### Getting Started

1. **Create a New Project**: Click "New Project" to start with a blank workspace
2. **Add Tracks**: Use the "+" button to add audio or MIDI tracks
3. **Record Audio**: Click the record button on an audio track and allow microphone access
4. **Create MIDI**: Double-click on a MIDI track to open the piano roll editor
5. **Apply Effects**: Click the "FX" button on any track to add effects
6. **Mix Your Project**: Adjust volumes and panning in the mixer section
7. **Export**: Click "Export" to render your project to an audio file

### Keyboard Shortcuts

- `Space`: Play/Pause
- `R`: Start/Stop Recording
- `Ctrl/Cmd + S`: Save Project
- `Ctrl/Cmd + O`: Open Project
- `Ctrl/Cmd + Z`: Undo
- `Ctrl/Cmd + Y`: Redo
- `Delete`: Delete selected items

### MIDI Controller Setup

1. Connect your MIDI controller to your computer
2. Click "Settings" > "MIDI Devices"
3. Select your controller from the list
4. Start playing!

## Requirements

- Modern web browser with support for:
  - Web Audio API
  - Canvas API
  - LocalStorage API
  - Web MIDI API (optional, for MIDI controller support)
  - MediaRecorder API (for audio export)
- Recommended browsers:
  - Chrome 90+
  - Firefox 88+
  - Edge 90+
  - Safari 14+

## Technology Stack

- **Web Audio API**: Real-time audio processing and synthesis
- **Canvas API**: High-performance waveform and piano roll rendering
- **Vanilla JavaScript**: No framework dependencies for maximum performance
- **CSS Grid/Flexbox**: Responsive, professional layout
- **LocalStorage API**: Persistent project storage
- **Web MIDI API**: External MIDI controller integration
- **MediaRecorder API**: Audio recording and export functionality

## Project Structure

```
ui-shout/
├── index.html          # Main application entry point
├── css/
│   ├── main.css        # Core styles
│   ├── mixer.css       # Mixer interface styles
│   ├── piano-roll.css  # Piano roll editor styles
│   └── sequencer.css   # Step sequencer styles
├── js/
│   ├── app.js          # Main application controller
│   ├── audio-engine.js # Web Audio API wrapper
│   ├── track.js        # Track management
│   ├── mixer.js        # Mixer logic
│   ├── piano-roll.js   # Piano roll editor
│   ├── sequencer.js    # Step sequencer
│   ├── effects.js      # Audio effects processors
│   ├── synth.js        # Software synthesizers
│   ├── midi.js         # MIDI handling
│   ├── recorder.js     # Audio recording
│   └── storage.js      # Project persistence
└── assets/
    ├── icons/          # UI icons
    └── samples/        # Demo audio samples
```

## Features in Detail

### Multi-track Recording
- Record from microphone or line input
- Non-destructive editing
- Waveform visualization
- Punch in/out recording

### MIDI Piano Roll
- Grid-based note editing
- Velocity editing
- Note quantization
- Copy/paste/duplicate functionality

### Step Sequencer
- 16-step patterns
- Multiple patterns per track
- Pattern chaining
- Velocity and probability per step

### Audio Effects
- Parametric EQ (3-band)
- Compressor/Limiter
- Reverb (convolution and algorithmic)
- Delay (stereo and ping-pong)
- Distortion/Overdrive
- Chorus/Flanger
- Filter (low-pass, high-pass, band-pass)

### Synthesizers
- Subtractive synthesizer
- FM synthesizer
- Sample-based playback
- ADSR envelope control
- LFO modulation

## Browser Compatibility

| Feature | Chrome | Firefox | Safari | Edge |
|---------|--------|---------|--------|------|
| Web Audio API | ✅ | ✅ | ✅ | ✅ |
| Canvas API | ✅ | ✅ | ✅ | ✅ |
| Web MIDI API | ✅ | ❌ | ❌ | ✅ |
| MediaRecorder | ✅ | ✅ | ✅ | ✅ |
| LocalStorage | ✅ | ✅ | ✅ | ✅ |

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Known Limitations

- Web MIDI API is not supported in Firefox and Safari
- Audio latency may vary depending on browser and operating system
- Projects are stored in LocalStorage (limited to ~5-10MB)
- Some audio effects may be CPU-intensive on older devices

## Future Enhancements

- Cloud project storage and collaboration
- VST plugin support via Web Assembly
- Advanced automation curves
- Video sync capabilities
- Mobile/tablet optimization
- Additional synthesizer types
- Sample library integration

## License

MIT License

Copyright (c) 2024 ui-shout

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Acknowledgments

- Built with the Web Audio API
- Inspired by professional DAWs like Ableton Live, FL Studio, and Logic Pro
- Special thanks to the web audio community

## Support

If you encounter any issues or have questions:
- Open an issue on GitHub
- Check the documentation in the `docs/` folder
- Join our community discussions

## Topics

`daw` `audio-workstation` `music-production` `midi-sequencer` `audio-recording` `web-audio` `synthesizer` `audio-effects`
