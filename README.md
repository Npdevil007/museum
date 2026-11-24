# Our Museum

An interactive 3D virtual museum built with vanilla JavaScript and Three.js. Designed as a digital space for preserving memories, displaying photographs, and creating an immersive personal experience through interactive exploration.

## Overview

**Our Museum** is a browser-based 3D environment where visitors can explore a virtual gallery, interact with displayed photographs, view multimedia content, and engage with objects within the environment.

The project combines lightweight 3D rendering with intuitive controls to create an accessible, interactive experience across desktop and mobile devices.

## Features

• Interactive 3D gallery environment  
• First-person exploration and camera controls  
• Keyboard-based movement  
• Touchscreen joystick for mobile navigation  
• Interactive photograph displays with dedicated viewing mode  
• Customizable image gallery and labels  
• Video display integration  
• Interactive seating functionality  
• Personalized visitor name display  
• Collision detection and movement boundaries  
• Responsive interface with safe-area support  
• Light and dark theme support  

## Tech Stack

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | Styling and responsive interface |
| JavaScript | Interaction and application logic |
| Three.js | 3D rendering and environment |

## Getting Started

### Prerequisites

• A modern web browser with WebGL support  
• Internet connection for loading Three.js from CDN  

### Installation

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/our-museum.git
```

Navigate to the project directory:

```bash
cd our-museum
```

Open `museum.html` in your browser to launch the application.

No build tools, package manager, or additional dependencies are required.

## Controls

| Action | Input |
|---|---|
| Move forward | W / Arrow Up |
| Move backward | S / Arrow Down |
| Move left | A / Arrow Left |
| Move right | D / Arrow Right |
| Look around | Click and drag |
| Mobile movement | On-screen joystick |
| Interact | Contextual action button |
| Exit viewing mode | Escape / Close |

## Configuration

The museum content can be customized directly from the configuration object inside `museum.html`.

### Personal Message

```javascript
message: {
  to: "For Emily",
  body: "Every photo here is a day I’d live again.",
  from: "— Alex"
}
```

### Photo Gallery

```javascript
photos: [
  { src: "images/photo1.jpg", label: "First trip" },
  { src: "images/photo2.jpg", label: "Our street" },
  { src: "images/photo3.jpg", label: "Sunday" },
  { src: "images/photo4.jpg", label: "The wedding" },
  { src: "images/photo5.jpg", label: "Home" },
  { src: "images/photo6.jpg", label: "Today" }
]
```

Images can be provided through local paths or externally hosted URLs. Leaving an image source empty automatically generates a placeholder.

### Video Display

```javascript
video: {
  src: "videos/our-film.mp4",
  label: "Our film"
}
```

A custom video can be added by providing its source path and display label.

## Project Structure

```text
our-museum/
├── museum.html
├── images/
│   ├── photo1.jpg
│   ├── photo2.jpg
│   └── ...
└── videos/
    └── our-film.mp4
```

The application currently runs as a standalone HTML file, making it easy to deploy and modify without a complex development environment.

## Technical Details

• Rendering powered by Three.js  
• Perspective camera and real-time rendering  
• Dynamic viewport resizing  
• Pointer-based camera controls  
• Keyboard and touch input handling  
• Collision detection and movement constraints  
• Canvas-generated placeholder textures  
• HTML video textures for multimedia display  
• Lightweight procedural environment construction  

## Roadmap

Potential future improvements:

- [ ] Custom 3D models and improved character animations
- [ ] Additional rooms and gallery environments
- [ ] More interactive objects
- [ ] Improved mobile controls
- [ ] Audio integration
- [ ] Saveable visitor progress
- [ ] Customizable museum layouts
- [ ] VR support

## License

This project is open source. Licensing terms can be defined according to the intended distribution and usage of the project.

---

Built with JavaScript and Three.js.
