# Maya_ZBrush_BlenderKeySet
A custom keyset for Blender that mimics Maya in Object and Edit modes and Zbrush in Sculpt mode.

Installation:
Go to Edit -> Preferences in Blender and find the Keymap tab. 
Click Import and import the included Industry_Compatible_Maya_ZBrush_VXX.py file. 

# 3D Viewport

### **1. Viewport Navigation & Manipulation**

- **Rotate View (Orbit)**:
    - `Alt + Left Mouse Button` (Press & Drag)
    - `Trackpad Pan` (Any direction) or `Mouse Rotate` (Any direction)
- **Pan View (Move Viewport)**:
    - `Alt + Middle Mouse Button` (Press & Drag)
    - `Wheel Left Mouse` / `Wheel Right Mouse`
    - `Shift + Trackpad Pan`
- **Zoom View**:
    - `Alt + Right Mouse Button` (Press & Drag)
    - `Wheel In` / `Wheel Out` (with or without `Alt`)
    - `Numpad +` / `Numpad -`
    - `Trackpad Zoom` or `Ctrl + Trackpad Pan`
    - `Mouse Smart Zoom` (Any direction)
- **Dolly View (Physical Camera Move)**: `Shift + Numpad +` / `Shift + Numpad -`
- **Smooth View Transition Animation**: Automatically handles viewport smoothing calculations via internal background triggers (`TIMER1`).

### **2. Framing & View Focus**

- **Frame Selected**: `F` (Focuses the viewport camera onto your active item/selection)
- **Center View on Pick Point**: `Shift + F` (Centers viewport around the specific pixel/coordinate clicked)
- **Frame All (Current Region)**: `A`
- **Frame All (All Available Screen Regions)**: `Shift + A`
- **Toggle Local View (Isolate Selection)**: `Shift + I` or `Ctrl + 1`

### **3. Cameras & Viewport Axis Orientations**

- **Toggle Camera View**: `F4`
- **Align to Major Axes**:
    - **Front View**: `F1` | **Back View**: `Ctrl + F1`
    - **Right View**: `F2` | **Left View**: `Ctrl + F2`
    - **Top View**: `F3` | **Bottom View**: `Ctrl + F3`
- **Orbit Right 180° (Flip View)**: `F5`

### **4. Advanced 3D Mouse Controls (NDOF / SpaceMouse)**

- **NDOF Orbit & Zoom**: Default 3D Mouse Motion
- **NDOF Orbit Only**: `Ctrl + 3D Mouse Motion`
- **NDOF Pan Only**: `Shift + 3D Mouse Motion`
- **NDOF All Axes Simultaneously**: `Shift + Ctrl + 3D Mouse Motion`
- **NDOF Button Hotkeys**:
    - **Frame Selected**: `NDOF Fit Button`
    - **Roll View Counter-Clockwise**: `NDOF Roll CCW Button` (Maps to left/right rolling)
    - **Orthographic snaps**: Dedicated NDOF Buttons (`Front`, `Back`, `Left`, `Right`, `Top`, `Bottom`)
    - **Align View to Active Element**: `Shift + NDOF Button` (Supports `Front`, `Right`, and `Top` variants)

### **5. Selection Controls (Left Mouse Click Modifications)**

- **Select & Clear Prior Selection**: `Left Mouse Click`
- **Toggle / Append Selection**: `Shift + Left Mouse Click`
- **Select Center / Target Object**: `Ctrl + Left Mouse Click`
- **Extend, Toggle, and Select Center**: `Shift + Ctrl + Left Mouse Click`
- **Enumerate Selection (Overlap Picker)**: `Shift + Alt + Left Mouse Click`
- **Enumerate Selection with Center Lock**: `Shift + Ctrl + Alt + Left Mouse Click`
- **Zoom Border Tool**: `Z` (Draw a box to zoom into a specific area)

### **6. Tool Windows, Menus, & Pie Menus**

- **Search Menu**: `TAB`
- **View Pie Menu**: `V`
- **Snap Pie Menu**: `Shift + X` or `Shift + Ctrl + Right Mouse Click Drag`
- **Pivot Point Pie Menu**: `Period (.)`
- **Transform Orientations Pie Menu**: `Comma (,)`

### **7. Modeling & Subdivision Surface Controls**

- **Set Subdivision Level 0**: `1` (Pressing removes or zeros out subdivision)
- **Set Subdivision Level 2 (Hide on Cage)**: `2` (Pressing sets subdivisions to level 2. *Releasing the key* explicitly turns off the "Show on Cage" option).
- **Set Subdivision Level 2 (Show on Cage)**: `3` (Pressing sets subdivisions to level 2. *Releasing the key* explicitly turns on the "Show on Cage" option).

### **8. Scene & Clipboard Utilities**

- **Translate (Move)**: `Left Mouse Click Drag` (Tweak action)
- **Toggle X-Ray Mode**: `Alt + X`
- **Toggle Snapping On/Off**: `X`
- **Copy Selection to Clipboard Buffer**: `Ctrl + C`
- **Paste Selection from Clipboard Buffer**: `Ctrl + V`
- **Toggle Screencast Keys Display Add-on**: `Shift + Alt + C`

### **9. 3D View Generic (UI Region Toggles)**

- **Toggle Toolbar UI Panel (T-Panel)**: `Ctrl + [`
- **Toggle Sidebar UI Panel (N-Panel)**: `Ctrl + ]` or `Ctrl + A`

# Object Mode

### **1. Timeline & Frame Navigation**

- **Step Forward / Backward 1 Frame**: `Right Arrow` / `Left Arrow`
- **Jump to Start / End of Timeline**: `Ctrl + Left Arrow` (Jump to first frame) | `Ctrl + Right Arrow` (Jump to last frame)

### **2. Object Selection & Hierarchy Controls**

- **Select All Objects**: `Shift + Ctrl + A`
- **Invert Selection**: `Shift + Ctrl + I`
- **Grow / Shrink Selection**: `Up Arrow` (Select More) / `Down Arrow` (Select Less)
- **Select Linked**: `Ctrl + L` (Selects objects sharing data or linked relationships)
- **Navigate Hierarchy (Parent/Child)**:
    - **Select Parent**: `[` (Left Bracket)
    - **Extend Selection to Parent**: `Shift + [`
    - **Select Child**: `]` (Right Bracket)
    - **Extend Selection to Child**: `Shift + ]`

### **3. Parenting & Collections**

- **Set Parent**: `P` (Establishes a parent-child relationship between selected objects)
- **Clear Parent**: `Shift + P` (Breaks the parenting relationship)
- **Move to Collection**: `Ctrl + G` (Opens the menu to move objects into a collection)
- **Link to Collection**: `Shift + Ctrl + G` (Links objects to an additional collection without moving them)

### **4. Visibility, Deletion & Duplication**

- **Hide Selection**: `H`
- **Hide Unselected (Isolate)**: `Shift + H`
- **Reveal Hidden Objects**: `Alt + H`
- **Delete Objects (Local)**: `Backspace` or `Delete`
- **Delete Objects (Global/All Scenes)**: `Shift + Backspace` or `Shift + Delete`
- **Duplicate & Move**: `Ctrl + D` (Duplicates the selected object and immediately activates the move tool)

### **5. Animation & Keyframing**

- **Insert Keyframe (LocRotScale)**: `S` (Instantly drops a location, rotation, and scale keyframe)
- **Insert Keyframe Menu**: `Shift + S` (Calls up the standard keyframe insertion dialogue)
- **Set Active Keying Set**: `Shift + Ctrl + Alt + S`

### **6. The QWERTY Layout & Active Tool Selection**

Pressing these keys cycles through the Left Toolbar active tool definitions:

- **`Q`**: Select Box Tool
- **`W`**: Move/Translate Gizmo
- **`E`**: Rotate Gizmo
- **`R`**: Scale Gizmo
- **`T`**: Combined Transform Gizmo
- **`D`**: Annotation/Grease Pencil Tool
- **`M`**: Measuring Tool
- **`C`**: 3D Cursor Placement Tool

### **7. Direct Transform Tool Overrides**

These actions override standard settings to immediately drop you into transform operations:

- **Direct Translate (Move)**: `Alt + W`
- **Direct Rotate**: `Alt + E`
- **Direct Resize (Scale)**: `Alt + R`

### **8. Interaction Mode Transitions (To Edit Mode)**

- **Enter Edit Mode (Default)**: `F8`
- **Enter Edit Mode + Vert Select**: `F9`
- **Enter Edit Mode + Edge Select**: `F10`
- **Enter Edit Mode + Face Select**: `F11`

### **9. Menus & Context Controls**

- **Object Menu**: `Right Mouse Click`
- **Add Object Menu**: `Shift + Right Mouse Click`
- **Object Context Menu**: `App Key` (Dedicated context menu key)
- **Object Mode Pie Menu**: `Right Mouse Click-Drag` (Gesture layout for quick mode switching)
- **Toggle Proportional Editing**: `B` (Turns object soft-transformation falloff on/off)

### **10. Explicitly Deactivated Hotkeys (`"active": False`)**

The following keys are mapped in the script but are turned off, meaning they will not execute:

- *Deselect All via `A`* (Disabled in favor of `Shift + Ctrl + A` behavior).
- *Clear Location/Rotation/Scale via `Alt + W`, `Alt + E`, `Alt + R`* (Disabled because these keybinds were converted to the Direct Transforms listed in Section 7).
- *Insert Specific Keyframes via `Shift + W / E / R`* (Disabled).
- *Delete Keyframe via `Alt + S`* (Disabled).
- *Right-Click Context Menu via `Right Mouse Press`* (Disabled; handled by `App Key`).
- *Edit Mode entry via numbers `1`, `2`, `3`* (Disabled; handled by `F9`, `F10`, `F11` instead).

# Mesh Editing

### **1. Mesh Loop & Path Selection**

- **Loop Select**: `Double Click Left Mouse` (Selects an edge, face, or vertex loop and clears prior selections)
- **Extend Loop Selection**: `Shift + Double Click Left Mouse` (Appends an additional loop to your selection)
- **Deselect Loop**: `Ctrl + Double Click Left Mouse` (Removes a loop from the current selection)
- **Shortest Path Pick (Edge Path)**: `Alt + Double Click Left Mouse` (Finds and selects the shortest path of components between two selections)
- **Shortest Path Pick (Region Fill)**: `Shift + Ctrl + Alt + Left Mouse Click` (Finds the shortest path and fills the enclosed regional area)

### **2. Component Selection Modes (Vertices, Edges, Faces)**

- **Direct Component Selection Switching**:
    - **Vertex Mode**: `F9`
    - **Edge Mode**: `F10`
    - **Face Mode**: `F11`
- **Extend Component Modes (Multi-Select Modes)**:
    - **Add Vertex Mode**: `Shift + 1`
    - **Add Edge Mode**: `Shift + 2`
    - **Add Face Mode**: `Shift + 3`*(Allows you to have combinations active simultaneously, e.g., Vertices and Edges active at once)*
- **Expand Selection Modes**: `Ctrl + 1` (Vertices), `Ctrl + 2` (Edges), `Ctrl + 3` (Faces)
- **Extend & Expand Selection Modes**: `Shift + Ctrl + 1` (Vertices), `Shift + Ctrl + 2` (Edges), `Shift + Ctrl + 3` (Faces)

### **3. Mesh Selection Utilities**

- **Select All Mesh Geometry**: `Shift + Ctrl + A`
- **Invert Current Selection**: `Ctrl + I`
- **Grow Selection (Select More)**: `Up Arrow` (Expands your selection outward to neighboring elements; repeatable)
- **Shrink Selection (Select Less)**: `Down Arrow` (Shrinks your selection inward from the borders; repeatable)
- **Select Linked Geometry**: `Ctrl + L` (Selects all contiguous geometry connected to the current selection)

### **4. Mesh Component Hiding & Visibility**

- **Hide Selection**: `H` (Conceals selected vertices/edges/faces)
- **Hide Unselected**: `Shift + H` (Isolates your selection by hiding everything else)
- **Reveal Hidden Mesh**: `Alt + H` (Unhides all concealed geometry within the active mesh)

### **5. Structural Editing & Geometry Deletion**

- **Mesh Duplicate & Move**: `Ctrl + D` (Duplicates the selected geometry and immediately activates the translation/move tool)
- **Delete Menu**: `Backspace` or `Delete` (Brings up the context-specific "Delete" options menu)
- **Dissolve Elements**: `Ctrl + Backspace` or `Ctrl + Delete` (Instantly dissolves selected geometry, cleanly merging the surrounding mesh structure)

### **6. The QWERTY Layout & Active Tool Selection**

Pressing these keys cycles through Blender's Left Toolbar active tool definitions:

- **`Q`**: Select Box Tool
- **`W`**: Move/Translate Gizmo
- **`E`**: Rotate Gizmo
- **`R`**: Scale Gizmo
- **`T`**: Combined Transform Gizmo
- **`D`**: Annotation/Grease Pencil Tool
- **`M`**: Measuring Tool
- **`C`**: 3D Cursor Placement Tool
- **`Ctrl + B`**: Bevel Tool
- **`I`**: Inset Faces Tool
- **`Ctrl + E`**: Extrude Region Tool
- **`K`**: Knife Topology Tool
- **`Alt + C`**: Loop Cut and Slide Tool

### **7. Direct Transform Tool Overrides**

These shortcuts bypass the toolbar gizmos to directly manipulate geometry:

- **Direct Translate (Move)**: `Alt + W`
- **Direct Rotate**: `Alt + E`
- **Direct Resize (Scale)**: `Alt + R`

### **8. Context Menus & Interaction Mode Toggles**

- **Mesh Select Mode Menu**: `Right Mouse Click` (Opens selection type filters)
- **Mesh Context Menu**: `Shift + Right Mouse Click` or `App Key` (Brings up context-sensitive modeling actions)
- **Main Edit Mesh Menu**: `Shift + Alt + Right Mouse Press`
- **Normals Menu**: `Alt + N` (Opens options to flip, recalculate, or reset vertex and face normals)
- **Object/Interaction Mode Pie Menu**: `Right Mouse Click-Drag` (Allows you to gesture out of Edit mode)
- **Toggle Mode Set**: `F8` (Switches interaction states)

### **9. Proportional Editing Controls**

- **Toggle Proportional Editing**: `B (Click)` (Turns soft selection falloff on or off)
- **Adjust Proportional Falloff Size**: `Hold B + Left Mouse Drag` (Triggers a radial adjustment tool to resize the soft-selection radius dynamically)

# Sculpt Mode

### **1. Core Sculpting Brush Strokes**

- **Standard Stroke**: `Left Mouse Press` (Applies the active brush normally)
- **Invert Brush Stroke**: `Alt + Left Mouse Press` (Flips the brush behavior, e.g., digging in instead of pulling out)
- **Smooth Brush Override**: `Shift + Left Mouse Press` (Temporarily switches the current brush to the Smooth brush)

### **2. Brush Properties & Radial Controls**

- **Adjust Brush Size**: `S` (Activates a radial controller to resize the brush radius)
- **Adjust Brush Strength**: `U` (Activates a radial controller to change stroke intensity)
- **Adjust Brush Hardness**: `Shift + S` or `O`
- **Adjust Texture Angle**: `Alt + S`
- **Adjust Mask Texture Angle**: `Ctrl + Alt + S`
- **Incremental Brush Scaling**: `[` (Scale down by 0.9x) | `]` (Scale up by 1.11x)
- **Toggle Lazy Mouse (Smooth Stroke)**: `L` (Toggles stabilizing your brush strokes)

### **3. Stencil & Texture Manipulation**

Using `Right Mouse` interactions allows you to transform your brush texture stencils in screen space:

- **Translate Stencil**: `Right Mouse Click-Drag`
- **Scale Stencil**: `Shift + Right Mouse Press`
- **Rotate Stencil**: `Ctrl + Right Mouse Press`

### **4. Masking Tools & Mask Expand**

- **Quick Toggle Mask Brush**: `A` (Press/Release switches into the default Mask brush tool)
- **Invert Mask**: `Ctrl + Left Mouse Click` (Flood-fills the opposite mask values)
- **Clear Mask**: `Ctrl + Alt + Left Mouse Click` (Clears the active mask completely)
- **Box Mask Gesture**: `Shift + Ctrl + Left Mouse Click-Drag` (Draws a box to apply a mask)
- **Box Unmask Gesture**: `Shift + Ctrl + Alt + Left Mouse Click-Drag` (Draws a box to erase a mask)
- **Lasso Mask Gesture**: `Ctrl + Left Mouse Click-Drag` (Draws a freehand selection to apply a mask)
- **Lasso Unmask Gesture**: `Ctrl + Alt + Left Mouse Click-Drag` (Draws a freehand selection to erase a mask)
- **Mask Expand (Geodesic)**: `Shift + A` (Expands a mask outward across topology from the cursor)
- **Mask Expand (Normals)**: `Shift + Ctrl + Alt + A` (Expands a mask based on face angles)
- **Mask Edit Pie Menu**: `Shift + Ctrl + A`
- **Auto-Masking Pie Menu**: `Shift + Alt + A`

### **5. Face Sets (Topology Grouping)**

- **Expand Face Set (Geodesic)**: `Shift + W` (Expands a face set outwards from under the cursor)
- **Expand Face Set (By Boundary)**: `Shift + Alt + W` (Expands until it hits an existing face set boundary)
- **Grow / Shrink Face Set**: `Page Up` / `Page Down`
- **Hide Active Face Set**: `H`
- **Toggle Face Set Visibility**: `Shift + H`
- **Face Sets Edit Pie Menu**: `Ctrl + W`

### **6. Mesh Visibility Controls**

- **Hide Masked Geometry**: `Ctrl + H` (Conceals parts of the mesh that are currently masked)
- **Unhide All Geometry**: `Alt + H` (Reveals all hidden parts of the mesh)

### **7. Subdivision Levels (Multires/SubD)**

- **Jump to Absolute Level**: `Ctrl + 0` through `Ctrl + 5` (Forces the subdivision modifier to a specific level)
- **Step Level Up (Relative)**: `D` (Increases the active sculpting resolution level by 1)
- **Step Level Down (Relative)**: `Shift + D` (Decrements the sculpting resolution level by 1)

### **8. Remeshing & Topology Utilities**

- **Voxel Remesh**: `Ctrl + M` (Executes a sharp voxel rebuild of the active mesh)
- **Edit Voxel Size**: `M` (Provides an on-screen preview to visually adjust target remesh density)
- **Dyntopo Detail Flood Fill**: `Ctrl + D`
- **Edit Dyntopo Detail Size**: `Shift + Ctrl + D`
- **Sample Mesh Color**: `I` or `C`

### **9. Tool Select & Direct Transforms**

Cycles or activates tools on the left shelf:

- **`Q`**: Paint/Sculpt Brush Tool
- **`W`**: Move Gizmo
- **`E`**: Rotate Gizmo
- **`R`**: Scale Gizmo
- **`T`**: Combined Transform Tool

### **10. Viewport Navigation & Menus**

- **Orbit View**: `Middle Mouse Click-Drag`
- **Pan View**: `Alt + Middle Mouse Click-Drag`
- **Zoom View**: `Ctrl + Middle Mouse Click-Drag`
- **Quick Axis Snapping (Gestures)**: `Shift + Middle Mouse Click-Drag` directional flick:
    - Flick **North** → Snap to Top View
    - Flick **East** → Snap to Right View
    - Flick **South** → Snap to Bottom View
    - Flick **West** → Snap to Left View
- **Toggle Symmetry (X-Axis)**: `X`
- **Toggle Perspective / Orthographic**: `P`
- **Sculpt Context Menu**: `Right Mouse Click` or `Spacebar` *(Note: The alternate `Right Mouse Click-Drag` object pie menu is disabled here).*
- **Quick Favorites / User Menu**: `Tab`
- **View Tools Pie Menu**: `Alt + Accent Grave (~)`
- **Sculpt Brush Asset Shelf Shelf**: `B` (Pops up a visual brush asset selection menu)
