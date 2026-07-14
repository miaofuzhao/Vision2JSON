# Vision2JSON

## A visual layout translator for AI-assisted development

A visual-to-structure protocol for AI-assisted development.

> 一个连接人类视觉表达与 AI 编程的轻量级布局转换工具。

**Turn visual ideas into structured data that AI coding agents can understand.**

Vision2JSON is a lightweight visual positioning and layout translation tool designed for people who use AI coding assistants to create games, apps, and interactive interfaces.

Instead of repeatedly telling AI:

> "Move this image a little to the right and make it smaller."

You can visually arrange your assets, adjust their position and size, then export precise JSON parameters that AI coding agents can understand.

---

# Changelog

## 2026-07-14

- Added image and video asset positioning support, allowing different media types to share the same layout protocol.
- Improved resolution-independent positioning using ratio-based coordinates.
- Enhanced AI-friendly JSON export for more accurate communication with AI coding agents.
- Added support for managing multiple visual layers with independent layout parameters.

## 2026-07-12

- Initial release with visual asset positioning workflow.
- Introduced ratio-based coordinates for resolution-independent layouts.
- Added AI-friendly JSON export to translate visual layouts into structured instructions for AI coding agents.
- Added support for managing multiple visual layers with independent position and size parameters.

---

# Why Vision2JSON?

AI coding assistants are becoming powerful enough to build applications and games, but there is still a communication gap:

**Humans think visually. AI needs structured parameters.**

Humans naturally understand:

> "Put this character near the bottom center."

But AI coding agents need structured information:

```json
{
  "layer": "character",
  "anchor": "bottom-center",
  "ratioPosition": {
    "x": 0.5,
    "y": 0.85
  },
  "ratioSize": {
    "width": 0.15,
    "height": 0.2
  }
}
```

Vision2JSON acts as a bridge between human visual intention and AI-generated code.

---

# Features

## Visual positioning

* Drag images and videos onto the canvas
* Move layers visually
* Resize assets with relative scaling
* Manage multiple layers
* Export structured layout information

---

## Resolution-independent coordinates

Traditional pixel coordinates break across different devices.

Vision2JSON uses relative coordinates:

```
0.0 ~ 1.0
```

Example:

```json
{
  "x": 0.5,
  "y": 0.5
}
```

always represents the center position of the canvas.

This allows layouts to adapt across:

* Mobile phones
* Tablets
* Desktop screens
* Different game resolutions

---

# Media positioning, not media understanding

Vision2JSON does not require AI agents to understand the internal content of images or videos.

The AI does not need to know:

* what object appears in the video;
* what the image represents;
* what animation happens inside the file.

It only needs structured layout information:

* Position
* Size
* Anchor point
* Layer order
* Rotation angle

The purpose of Vision2JSON is to describe **where and how an asset should exist inside an application**.

---

# AI-friendly JSON export

Export structured layout information:

```json
[
  {
    "layer": "Image 2",
    "visible": true,
    "anchor": "top-left",
    "ratioPosition": {
      "x": 0.5,
      "y": 0.5
    },
    "ratioSize": {
      "width": 0.1455,
      "height": 0.2183
    },
    "rotation": 0,
    "zIndex": 2
  }
]
```

The exported data can be provided directly to:

* AI coding agents
* Game development assistants
* UI generation workflows

---

# Use Cases

## AI game development

When creating games with AI assistants:

Instead of manually describing:

* character positions
* buildings
* trees
* buttons
* dialog windows
* visual effects

You can arrange assets visually and provide exact layout data to AI.

---

## AI application development

Useful for:

* H5 pages
* Web applications
* Mobile interfaces
* Interactive prototypes
* AI-assisted UI generation

---

# How to use

1. Open `index.html` in your browser.
2. Drag your background image or video into the canvas.
3. Add additional assets.
4. Adjust position, size, and layer order.
5. Copy the generated JSON.
6. Send the layout information to your AI coding assistant.

No installation required.

No dependencies.

Runs completely locally in your browser.

---

# Design philosophy

Vision2JSON is built around a simple idea:

> In the AI era, the bottleneck is not only writing code. It is expressing ideas precisely.

This project explores a new workflow:

```
Human visual intention
          ↓
Visual editor
          ↓
Structured specification
          ↓
AI-generated implementation
```

---

# Technology

Built with:

* Pure HTML
* CSS
* JavaScript

No frameworks.

No build tools.

Just open and use.

---

# Roadmap

Possible future improvements:

* Import JSON and restore layouts
* Rotation controls
* Layer ordering management
* More anchor point options
* Timeline and interaction recording
* Export formats for different engines

Potential integrations:

* Unity
* Godot
* Web frameworks

---

# Author

Miao Fuzhao

Email:
miao.fuzhao.research@gmail.com

Independent AI-assisted creator exploring human-AI collaboration.

---

# Origin

This project was created while building AI-assisted games and applications.

During development, I found that describing visual layouts to AI coding agents often required many rounds of manual adjustment.

Vision2JSON was created to reduce the communication gap between human creativity and AI implementation.

---

# License

MIT License

Copyright (c) 2026 Miao Fuzhao
