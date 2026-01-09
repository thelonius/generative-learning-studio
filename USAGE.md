# Generative Learning Studio - Usage Guide

## Quick Start

1. **Open the Application**
   - Open `index.html` in a modern web browser (Chrome, Firefox, Edge, Safari)
   - Or serve it with: `python -m http.server 8000` and visit `http://localhost:8000`

2. **Choose a Pattern**
   - Click buttons to select different generative patterns:
     - **L-Systems** - Plant-like structures
     - **Mandelbrot** - Famous fractal zoom
     - **Sierpinski** - Triangle fractal
     - **Perlin Noise** - Organic landscapes

3. **Adjust Parameters**
   - **Speed**: Control animation speed (0.1x - 2x)
   - **Detail**: Set recursion/iteration depth (1-8 levels)
   - **Color Scheme**: Choose from 5 palettes (Neon, Nature, Ocean, Fire, Mono)
   - **Scale**: Zoom in/out (0.5x - 3x)

## Voice Commands

### Activation
- Click the **microphone button** or press **Space** to start voice recognition
- The status will show "Listening..."

### Supported Commands

#### Pattern Selection
- "растение" / "plant" → Switch to L-Systems
- "фрактал" / "fractal" → Switch to Mandelbrot
- "треугольник" / "triangle" → Switch to Sierpinski  
- "шум" / "noise" → Switch to Perlin Noise

#### Control Commands
- "старт" / "start" / "играй" / "play" → Start animation
- "стоп" / "stop" / "пауза" / "pause" → Pause animation
- "сброс" / "reset" → Reset all parameters
- "случайно" / "random" → Random generation

#### Parameter Adjustments
- "быстрее" / "faster" → Increase speed
- "медленнее" / "slower" → Decrease speed
- "больше деталей" / "more detail" → Increase detail level
- "меньше деталей" / "less detail" → Decrease detail level
- "увеличить" / "zoom in" → Zoom in
- "уменьшить" / "zoom out" → Zoom out

#### Color Schemes
- "неон" / "neon" → Neon color palette
- "природа" / "nature" → Nature colors
- "океан" / "ocean" → Ocean blues
- "огонь" / "fire" → Fire/warm colors
- "моно" / "mono" → Monochrome

#### AI Explanations
- "объяснить" / "explain" → Get AI explanation of current pattern
- "что это" / "what is this" → Describe current visualization

## Controls

### Buttons
- **Play/Pause** (▶/⏸) - Toggle animation
- **Reset** (🔄) - Reset to default settings
- **Random** (🎲) - Generate random pattern
- **Microphone** (🎤) - Activate voice control

### Keyboard Shortcuts
- **Space** - Toggle voice recognition
- **P** - Play/Pause animation
- **R** - Reset parameters
- **1-4** - Quick pattern selection
- **Arrow Up/Down** - Adjust speed
- **Arrow Left/Right** - Adjust detail level

## Patterns Explained

### L-Systems (Lindenmayer Systems)
**What**: Formal grammars that model plant growth
**Rules**: Each symbol is replaced according to production rules
**Example**: `F` → `F+F--F+F` creates branching structures
**Use Cases**: Plants, trees, organic patterns, procedural generation

### Mandelbrot Set
**What**: Mathematical fractal defined by iterating z² + c
**Properties**: Self-similar at all scales, infinite detail
**Colors**: Represent iterations to escape or stay bounded
**Use Cases**: Fractals, chaos theory, beautiful mathematical art

### Sierpinski Triangle
**What**: Recursive triangle subdivision
**Process**: Remove central triangle, repeat on remaining triangles
**Dimension**: ~1.585 (between 1D line and 2D plane)
**Use Cases**: Fractals, recursion learning, geometric art

### Perlin Noise
**What**: Gradient noise function for natural-looking randomness
**Properties**: Smooth, continuous, controllable frequency
**Invented**: By Ken Perlin (1983) for Tron movie
**Use Cases**: Terrain generation, clouds, textures, procedural content

## Statistics

### Real-time Metrics
- **FPS Counter**: Shows current frames per second
- **Element Count**: Number of objects being rendered
- **Voice Commands**: Displays last recognized command

## Tips & Tricks

1. **Performance Optimization**
   - Lower detail level if FPS drops below 30
   - Reduce scale for complex patterns
   - Pause when adjusting multiple parameters

2. **Best Visual Results**
   - Try different color schemes with each pattern
   - Combine slow speed with high detail for intricate views
   - Use Random button to discover interesting combinations

3. **Learning Mode**
   - Use "explain" voice command to learn about patterns
   - Experiment with detail levels to see recursion in action
   - Compare different patterns at same detail level

4. **Creative Exploration**
   - Screenshot interesting moments (browser's screenshot tool)
   - Try extreme parameter values
   - Combine voice and manual controls for fluid workflow

## Browser Compatibility

### Fully Supported
- ✅ Chrome/Edge 90+
- ✅ Firefox 88+
- ✅ Safari 14+

### Features by Browser
- **Voice Recognition**: Chrome/Edge (best), Firefox (limited), Safari (requires permission)
- **Canvas Rendering**: All modern browsers
- **Web Speech API**: Chrome/Edge (excellent), Firefox (basic), Safari (basic)

## Troubleshooting

### Voice Control Not Working
- **Check microphone permissions** in browser settings
- **Use HTTPS or localhost** (required for Web Speech API)
- **Speak clearly** with minimal background noise
- **Try Chrome/Edge** for best voice recognition

### Low FPS / Laggy Animation
- **Reduce detail level** (try 3-4 instead of 7-8)
- **Lower scale** to 1x or below
- **Close other browser tabs** consuming resources
- **Update graphics drivers**

### Pattern Not Displaying
- **Check browser console** (F12) for errors
- **Refresh the page** (Ctrl+R / Cmd+R)
- **Try a different browser**
- **Clear browser cache**

### AI Explanations Not Working
- This feature requires **LLM API integration** (optional)
- Currently shows **pre-written descriptions**
- For live AI: Add OpenAI/Google API key in future version

## Advanced Usage

### Customization
Edit `index.html` to:
- Add new L-System rules
- Modify color palettes
- Adjust default parameters
- Create custom patterns

### API Integration (Future)
- Connect to external LLM for dynamic explanations
- Send voice commands to Grasshopper/TouchDesigner
- Export patterns as SVG/PNG
- Save/load custom presets

## Educational Use

### For Students
- Learn about recursion and fractals
- Understand procedural generation
- Explore mathematical beauty
- Practice voice-controlled interfaces

### For Teachers
- Demonstrate L-systems and formal grammars
- Show fractal geometry concepts
- Teach human-computer interaction
- Integrate with computational art curriculum

### For Developers
- Study Canvas API usage
- Learn Web Speech API integration
- Understand generative algorithms
- See real-time rendering techniques

## Resources

- [L-Systems Wikipedia](https://en.wikipedia.org/wiki/L-system)
- [Mandelbrot Set Explorer](https://mathworld.wolfram.com/MandelbrotSet.html)
- [Perlin Noise Tutorial](https://adrianb.io/2014/08/09/perlinnoise.html)
- [Web Speech API Docs](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API)

## Credits

Created as an interactive learning tool for generative art and computational design.
Inspired by mathematical beauty and parametric modeling tools like Grasshopper.

---

**Have fun exploring generative patterns! 🎨✨**
