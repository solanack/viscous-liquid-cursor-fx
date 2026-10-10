# Enhanced Viscous Liquid - Cursor FX

This project is a reverse-engineered and feature-enhanced version of the "Viscous Liquid - Cursor FX" CodePen by @sabosugi (https://codepen.io/editor/sabosugi/pen/01a125aa-40e8-70ca-b198-550dc149d263).

## Original Concept
A Three.js / WebGL full-screen shader effect simulating viscous liquid that reacts to cursor movement. Typical of sabosugi's free source code pens using custom GLSL for fluid-like interactions.

## Reverse Engineering Notes
- Full-screen orthographic plane with custom ShaderMaterial.
- Fragment shader using FBM noise for liquid patterns.
- Mouse position drives flow influence with viscosity-based damping.
- Time-based animation for organic motion.

## Added Features
Using concepts from motion/animation repositories (solanack/motion, remotion, motion-graphics, etc.):

- **Interactive Controls**: Real-time sliders for viscosity, flow speed, and cursor strength. Color scheme selector (Neon, Gold, Cyber).
- **Smoothed Cursor Interaction**: Lerp-based mouse following for more viscous, laggy liquid response.
- **UI Overlay**: Semi-transparent control panel (can be animated further with Motion library).
- **Extensibility**:
  - Easy to wrap in a Remotion composition for programmatic video export.
  - Overlay elements can use the Motion (Framer Motion successor) library for spring-based UI animations.
  - Compatible with GSAP timelines if preferred from motion-graphics skills.
  - Potential for multi-layer or particle enhancements drawing from animate/hyperframes repos.

## Usage
Open `index.html` in a modern browser. Move the mouse to interact with the liquid.

To integrate with your repos:
1. Copy the shader logic into a Remotion component for video generation.
2. Use Motion's `animate` for control panel transitions.
3. Extend with skills from `awesome-motion-design-agent-skills` or `claude-motion-design` for agent-assisted further enhancements.

## Dependencies
- Three.js (loaded via CDN)
- No other external deps for the core effect

## License Note
Original sabosugi source codes are free for use. This enhanced version follows the same spirit.