# displaypak
Electron/Tauri are bloat fr, I want LIGHTWEIGHT and SIMPLE package for rendering interactable UI elements to a window

The window is composed of a tree of **components**. There are two types of component:
- **Regions** - Basically a flexbox (with all your standard flexbox properties, a background color, padding, and boolean controlling whether it is shown or not) that can contain other components.
- **Elements** - Text, images/textures, buttons, text input, and so forth.

`create_region(parent region or null, properties) => region object`

`component_set_parent(parent region or null, child component) => void`

`set_window_region(region) => void`

The **window region** is just the region that takes up the entire space of the window, which all other elements are displayed within.

There's no single `create_element` function because each type of element is initialized differently.

Popovers/modals do not exist.
