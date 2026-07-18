# displaypak
A LIGHTWEIGHT and SIMPLE Electron/Tauri alternative for rendering interactable UI elements to a single window.

The window is composed of a tree of **components**. There are two types of component:
- **Regions** - Basically a flexbox (with all your standard flexbox properties, a background color, padding, and boolean controlling whether it is shown or not) that can contain other components. One region at any given time is designated as the **window region,** which takes up the entire space of the window, and which all other elements are displayed within.
- **Elements** - Everything that's not a region. Text, images/textures, buttons, text input, and so forth.

`create_region(parent region or null, properties) => region object`

`component_set_parent(parent region or null, child component) => void`

`set_window_region(region) => void`

`create_text_element(string) => component`

Popovers/modals do not exist.
