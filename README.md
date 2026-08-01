# Kinship Chart Builder

A single, self-contained web page for building genealogical / kinship charts using standard notation, then exporting them as a PNG image.

Just open `kinship-chart-builder.html` in any modern desktop web browser (Chrome, Edge, Firefox, or Safari). No internet connection, installation, or extra files are required. It is a desktop tool driven by the mouse, so it does not work well on phones or tablets.

> **Tip:** Click the **? Instructions** button in the top toolbar to see this same guide inside the app at any time.

## Notation

- **Triangle** = male
- **Circle** = female
- **Square** = unknown sex
- A **diagonal line through a symbol** = deceased
- **Double line** between two people = marriage
- **Double line with a single slash** = divorce / separation
- **Dashed line** = partnership
- **Vertical drop from a couple's union line to a horizontal bar** = their children
- **Colors** are optional and mean whatever you define in the legend

## Adding people

- **Add a person:** drag a symbol from the *People* palette onto the canvas. It snaps to the grid.
- **Name a person:** double-click the symbol and type their name.
- **Mark deceased:** right-click a person and choose *Add deceased slash*.
- **Default shape color:** right-click a symbol in the palette to set a default fill for every new person of that type.

## Relationships

There are two ways to connect people.

**1. Using the sidebar buttons**

- Click a relationship button (or press <kbd>M</kbd> for marriage, <kbd>P</kbd> for partnership), then click the two people.
- For *Parent → child*, click the couple's union line (or a single parent), then click the child. Multiple children of one couple share a single descent line and sibling bar.

**2. Shift-drag directly on the canvas**

- <kbd>Shift</kbd> + drag one person onto another = marriage.
- <kbd>Shift</kbd> + drag a union line onto a person = that person becomes a child.
- <kbd>Shift</kbd> + drag to empty space = a small menu asks which shape to create; it is placed there and connected (spouse from a person, child from a union line).

Other relationship actions:

- **Divorce:** right-click a marriage line and choose *Add divorce slash*.
- **Delete a link:** right-click any line and choose *Delete link*.

## Selecting & moving

- **Select:** left-click a person or line.
- **Add/remove from a selection:** <kbd>Shift</kbd> + click a person.
- **Box-select:** left-drag across empty space to select everyone inside the box.
- **Move:** drag a selected person. A multi-selection moves together, and connector lines follow.
- **Delete:** press <kbd>Delete</kbd> or <kbd>Backspace</kbd>.
- **Cancel / clear:** press <kbd>Esc</kbd> (cancels a link in progress or clears the selection).

## Colors & legend

- **Define colors:** in the *Colors* panel, click *+ Add color* to add color + label rows. Click the color chip to change the color, type a label, and use the **×** to remove it (it asks for confirmation if that color is currently in use).
- **Apply a color:** select one or more people, then click a swatch in the *Selected* panel — or right-click a person and pick a color.
- **Legend:** turn on *Legend in PNG* to include a key in the exported image. The legend lists only the symbols, line types, and colors you actually used.

## Navigating the canvas

The canvas is an infinite pan/zoom surface.

- **Pan:** right-click and drag on empty space.
- **Zoom:** scroll wheel (zooms toward the cursor).
- **Center:** press <kbd>Space</kbd> to center the view on your chart.
- **Fit:** press <kbd>Enter</kbd> to zoom so the whole chart fits on screen.

## Saving & exporting

- **Save JSON:** downloads the entire chart (people, links, colors, and defaults) so you can keep editing it later.
- **Load JSON:** restores a saved chart. Files saved by older versions are automatically migrated on import.
- **Export PNG:** saves a high-resolution image cropped to your chart, with the legend included if *Legend in PNG* is enabled.

## Other toolbar controls

- **Snap to grid:** toggles grid snapping when placing/moving people.
- **Show grid:** toggles the background grid (also affects the PNG).
- **Load sample:** loads an example family so you can see the conventions.
- **Clear:** removes everything from the canvas (asks first).

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| <kbd>M</kbd> | Start a marriage link |
| <kbd>P</kbd> | Start a partnership link |
| <kbd>Space</kbd> | Center the view on the chart |
| <kbd>Enter</kbd> | Zoom to fit the whole chart |
| <kbd>Delete</kbd> / <kbd>Backspace</kbd> | Delete the current selection |
| <kbd>Esc</kbd> | Cancel linking / clear selection (or close the Instructions popup) |
| <kbd>Shift</kbd> | Hold while clicking/dragging for multi-select and quick linking |
