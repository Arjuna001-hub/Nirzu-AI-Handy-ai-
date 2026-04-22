# Handy AI – Gesture Intelligence Platform

## Overview

An immersive web-based AI application that uses your camera to track hand gestures in real-time, enabling three interactive modes: **Play** (particle effects), **Shapes** (draw symbolic shapes), and **Write** (air drawing).

## Live Demo

Open `Nirzu.html` in a modern browser (Chrome/Edge recommended). Camera access is required.

---

## Features

### 🎮 Play Mode
- **Pinch** (thumb + index) → Fire shockwave ripple + particle burst
- **Two hands** → Lightning arcs between fingertips + rotating mandala
- **Fast movement** → Accelerates the Matrix-style rain background

### 🔷 Shapes Mode
- **Heart** – Bring both palms close with fingers open
- **Peace sign** – Extend index + middle fingers, curl others
- **Star Burst** – Make fists with both hands

### ✍️ Write Mode
- **Point index finger** → Draw glowing neon lines in the air
- **Pinch** → Lift pen (stop drawing)
- **Shake open palm rapidly** → Clear the canvas (visual progress ring shows shake intensity)

---

## Controls

| Element | Action |
|---------|--------|
| **Top bar** | Mode switcher (Play / Shapes / Write) |
| **Clear Canvas** | Button in bottom-right (Write mode only) |
| **Shake gesture** | Open palm → shake left/right → clears canvas (Write mode) |

---

## Technical Stack

- **MediaPipe Hands** – 21-point hand landmark tracking
- **HTML5 Canvas** – Real-time rendering with particle system
- **Web Audio API** – Gesture-triggered sound effects
- **CSS Backdrop Filters** – Glass-morphism UI

---

## System Requirements

- **Browser:** Chrome, Edge, or any WebRTC-compatible browser
- **Camera:** Front-facing camera required
- **Lighting:** Good lighting improves detection accuracy
- **Performance:** Dedicated GPU recommended for smooth 30fps

---

## Gesture Reference

| Mode | Gesture | Visual Feedback |
|------|---------|-----------------|
| Play | Pinch | Ripple + particle explosion + zap sound |
| Play | Two hands | Lightning arcs, rotating mandala, ambient hum |
| Shapes | Heart | Animated glowing heart with gradient |
| Shapes | Peace | Circle with peace symbol |
| Shapes | Fists both | Rotating star burst |
| Write | Index point | Neon cursor + drawing trail |
| Write | Pinch | Pen lift |
| Write | Shake open palm | Ring progress meter → canvas clears |

---

## File Structure

```
Nirzu.html          # Single-file application (HTML/CSS/JS)
```

No build step or dependencies required – runs directly in browser.

---

## Known Limitations

- Requires `https` or `localhost` for camera access in some browsers
- Performance may degrade on low-end devices
- Gesture detection works best with clear hand visibility against a plain background
- Audio context requires user interaction (enabled after clicking "Enter Experience")

---

## Credits

Built with MediaPipe, Canvas API, and Web Audio API.
