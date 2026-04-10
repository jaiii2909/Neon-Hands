# 🌌 Neon Hands

A high-performance, real-time AI air drawing web application built around advanced hand tracking and spatial gestures.

Draw with your dominant hand while the secondary hand manipulates strokes in real time using Move, Scale, and Rotate controls.

## ✨ Key Features

*   **✋ Dual-Hand Interaction**
    *   **Right Hand (Dominant)**: High-precision drawing, selective erasing, and canvas clearing.
    *   **Left Hand (Secondary)**: Spatial transforms for existing strokes: Move, Scale, and Rotate.
*   **📐 Non-Destructive Transforms**
    *   Strokes preserve original coordinates, while translation, scaling, and rotation are applied at render time using matrix math.
*   **🕶️ Glassmorphism UI**
    *   Clean neon-inspired interface with real-time HUD cues and gesture feedback.
*   **⚡ Smooth Performance**
    *   Optimized rendering for fluid interaction and responsive motion.
*   **🌀 Physics-Inspired Behavior**
    *   Intuitive inertia for stroke movement and 45° rotation snap points.
*   **📖 Built-In Gesture Guide**
    *   Helps users learn the control scheme without leaving the app.

## 🛠️ Tech Stack

*   **Frontend**: React + Vite
*   **Hand Tracking**: @mediapipe/hands
*   **Animations**: Framer Motion
*   **Icons**: Lucide React with inline SVG fallbacks
*   **Styling**: Vanilla CSS with modern glassmorphism and neon accents

## 🎮 Gesture Manual

### ✍️ Drawing Hand (Right Hand)
| Gesture | Action |
|---|---|
| ☝️ **Index Up** | Start drawing a stroke |
| 🤏 **Pinch** | Erase selectively along fingertip path |
| ✊ **Fist** | Clear the entire canvas |

### 🖐️ Control Hand (Left Hand)
| Gesture | Action | Feedback |
|---|---|---|
| ✌️ **Two Fingers** | Move the nearest stroke | Blue crosshair + glow |
| 🤏 **Pinch & Spread** | Scale the selected stroke | Concentric rings + percentage label |
| 🤚 **Open Palm** | Rotate the stroke | Orange arc with snap indicators |

## 🚀 Getting Started

1.  Install dependencies:
    ```bash
    npm install
    ```
2.  Launch the development server:
    ```bash
    npm run dev
    ```
3.  Grant camera access and place your hands in view.


