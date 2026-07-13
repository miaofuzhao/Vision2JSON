# Vision2JSON

## A visual layout translator for AI-assisted development
> 一个连接人类视觉表达与 AI 编程的轻量级布局转换工具。
**Turn visual ideas into structured data that AI coding agents can understand.**

Vision2JSON is a lightweight visual positioning tool designed for people who use AI coding assistants to create games, apps, and interactive interfaces.

Instead of repeatedly telling AI:

> "Put this image a little more to the right and make it smaller."

You can simply drag, resize, and position the asset visually — then export precise JSON parameters for your AI coding workflow.

---

## Why Vision2JSON?

AI coding assistants are becoming powerful enough to build applications and games, but there is still a communication gap:

**Humans think visually. AI needs structured parameters.**

For example:

Human:

> "Place this character in the center-bottom of the scene."

AI needs something like:

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

Vision2JSON acts as the bridge between human visual intention and AI-generated code.

---

# Features

## Visual positioning

* Drag images and videos onto the canvas
* Move layers visually
* Resize assets with resolution-independent scaling
* Manage multiple layers

## Resolution-independent coordinates

Instead of fixed pixels, Vision2JSON uses relative coordinates:

```
0.0 ~ 1.0
```

This allows layouts to work across:

* Mobile phones
* Tablets
* Desktop screens
* Different game resolutions

Example:

```json
{
  "x": 0.5,
  "y": 0.5
}
```

always means the center of the canvas.

---

## AI-friendly JSON export

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

The output can be directly provided to:

* AI coding agents
* Game development assistants
* UI generation workflows

---

# Use Cases

## AI game development

Example:

You are creating a farming game with AI.

Instead of manually adjusting:

* trees
* animals
* buildings
* buttons
* dialog windows

You can visually arrange them and give AI the exact layout data.

---

## AI application development

Useful for:

* H5 pages
* Web applications
* Mobile interfaces
* Interactive prototypes

---

# How to use

1. Open `index.html` in your browser.
2. Drag your background image into the canvas.
3. Add additional assets.
4. Adjust position and size.
5. Copy the generated JSON.
6. Send the layout information to your AI coding assistant.

No installation required.

No dependencies.

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
* Export formats for different engines

  * Unity
  * Godot
  * Web frameworks

---

# Author

Miao Fuzhao

Independent AI-assisted creator exploring human-AI collaboration.

---

# Origin

This project was created while building AI-assisted games and applications.

During development, I found that describing visual layouts to AI coding agents often required many rounds of manual adjustment.

Vision2JSON was created to reduce this communication gap.

---

# License

MIT License

Copyright (c) 2026 Miao Fuzhao
