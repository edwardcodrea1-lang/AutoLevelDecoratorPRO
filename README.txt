Auto Level Decorator PRO — README
A powerful Unity Editor tool for fast level decoration using scatter areas and a real‑time brush system.
Designed for speed, flexibility, and clean workflows.

📦 Installation
Download the .unitypackage

Import it into your Unity project

The tool will appear under:
Tools → Auto Level Decorator PRO

Make sure the script is inside:
Assets/Editor/

🧰 Features
Scatter objects inside rectangular areas

Real‑time brush painting (hold LMB)

Dynamic spawn rate (faster when moving the mouse)

Adjustable brush strength, radius, density

Slope filtering

Layer filtering

Tag filtering

Random scale + rotation

Parent assignment

SceneView gizmos (brush circle + scatter area outlines)

🚀 Quick Start
1. Assign Prefabs
Drag your prefabs into the Prefabs list.
(Use real prefab assets from the Project window.)

2. Create a Parent
Create an empty GameObject (optional):
Right‑click → Create Empty → "DecoratedLevel"

Assign it to the Parent field.

3. Scatter Mode
Add a scatter area

Adjust:

Center

Size

Count

Click Scatter All Areas

Objects will spawn inside the green rectangle.

4. Brush Mode
Enable Brush Mode

Set:

Radius

Density

Strength

Hold Left Mouse Button in Scene View

Move the mouse to paint objects continuously

The yellow circle shows the brush area.

⚙️ Customization
Spawn Rules
Setting	Description
Y Offset	Lifts objects above the ground
Min Distance	Prevents overlapping
Max Slope Angle	Blocks steep terrain
Align To Slope	Rotates objects to match terrain
Allowed Layers	Only spawn on selected layers
Allowed Tags	Only spawn on objects with specific tags


Randomization
Setting	Description
Scale Range	Random uniform scale
Random Y Rotation	Random rotation around Y axis


Brush Settings
Setting	Description
Radius	Brush size
Density	Objects per stroke
Strength	Spawn speed multiplier


🛠 Debugging
❗ Prefabs not spawning
Make sure you assigned real prefab assets, not scene objects

Check that your ground has a Collider

Ensure Allowed Layers includes your terrain

Check Max Slope Angle (set to 90 to test)

❗ Layer index out of bounds
Reset Allowed Layers to “Default”.
This happens when Unity serializes invalid bits.

❗ Nothing spawns in Brush Mode
Make sure Brush Mode is enabled

Hold Left Mouse Button

Move the mouse (spawn rate increases with movement)

Check brush radius > 0.1

Check prefabs list is not empty

❗ Objects spawn too fast / too slow
Adjust:

Brush Strength

Brush Density

Min Distance

❗ Gizmos not visible
Enable:
Gizmos → On in Scene View.

📌 Tips
Use a Parent object to keep your hierarchy clean

Use Min Distance to avoid clutter

Use Brush Strength for fast mass‑painting

Use Scatter Areas for large‑scale placement

Use Tags to restrict spawning to specific surfaces

Use Align To Slope for rocks, OFF for trees

🧩 Requirements
Unity 2021+

Any render pipeline

Terrain or mesh with colliders

Prefabs with meshes

📄 License
You may use this tool in personal and commercial projects.
Redistribution or resale of the tool itself is not allowed unless permitted by the author.