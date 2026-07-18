# displaypak
Electron/Tauri are bloat fr, I want LIGHTWEIGHT and SIMPLE package for rendering interactable UI elements to a window

The window is composed of a tree of **components**. There are two types of component:
- **Areas** - Basically a flexbox (with all your standard flexbox properties, a background color, padding, and boolean controlling whether it is shown or not) that can contain other components.
- **Elements** - Text, images/textures, buttons, text input, and so forth.

The function that creates an area inputs its properties + the parent area and outputs an area object (which you can call another function on to add a component to it). There is also an additional function for setting an area as the 'main window area' (an area that takes up the entire space of the window).

**popovers do not exist. they're BLOAT**
