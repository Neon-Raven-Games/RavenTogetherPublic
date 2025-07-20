# Raven Together™ ![qt](/RT.png)
> Raven Together – A next-gen pixel art editor built for artists, powered by code, and designed for multiplayer creativity from the ground up.
No bloat. No waiting. Just real-time collaboration, editable tiles, and shader hot reloads. Built solo. Ready to scale.

## 💡 Help Push This Further
Built on nothing but desperation and code. Help me survive, for everyone tired of bloated engines and broken pipelines.

🎥 [See it in Action](https://youtu.be/aicetnL96HU) <br>
☕ [Support on Ko-Fi](https://ko-fi.com/neonraven3)

Even $5 keeps the lights on. Literally.

*“Neon Raven™ and Raven Together™ are the ongoing works of Michael Ross. All rights reserved. Unauthorized use prohibited.”*
> 🚧 Still cleaning up. Full docs and demo incoming. Raven Together is the first public-facing phase of a much larger vision. It starts with pixel art, but it doesn’t end there.

## User Testimony
- "… but it looks so continuous. Like didn’t you close the software once?"
- " The dynamic aspect where the changes happen to all the blocks was cool"
- "This is really cool.  I love the concept of painting with pre-designed squares so you could make stuff with like a palette of textures instead of just a palette of colors. "
- "this just gives me a lot of cool ideas, as someone that's not super familiar with working on pixel art."

| Features               | Digitizer           | Unity      | Godot        | RPG maker |
|------------------------|---------------------|------------|--------------|-----------|
| Network First Design   | ✅                   | ❌          | ❌            | ❌         |
| Real-Time Sprite Edits | ✅                   | ❌          | ❌            | ❌         |
| Hot Reload Shaders     | ✅ Shader DSL        | ⚠️ Partial | ✅ (manual)   | ❌         |
| DSL & Scripting Engine | ✅ Compiled and Live | ❌          | ✅ (GDScript) | ❌         |

> 🛠️ Built from scratch, almost died for it. If it resonates, [send food](https://ko-fi.com/neonraven3).

## 🧭 Philosophy
- Built by someone who's been crushed by the world and bad engines. This one fights back. No bloat. No lies. Just creation.
- Creativity is full of happy mistakes and tools should enhance creative flow not adhere to a user's vision. Think Bob Ross and the happy tree.
- Creative Flow > Unlimited inclusion
- I write everything from scratch, so I can be confident when I slap my name on it. Currently, only monogame exists (porting to vulkan with your help <3)

## Feature Lifecyles
- Functionality - Make it work, make it work good
- Scalability - Make it go hard or go home
- Portability - Isolate any rendering logic introduced outside what I personally wrote
- Usability - UX and scalability within the UX, better known as "Polish"

## General
- An editor that doesn't *just* work, it looks and *feels*.
- Use textures as a palette, or colors to design textures.
- Fluid and seamless work without context switching between apps.
- Edit one tile, edit your world. 
- Bloat-free performant art/design first engine with extensibility expected by developers
- Network First Design: written with a collaboration focus from the ground up 
- Prototype phase - Art and level creation pipeline to data export
- Designed for production, scales by default.
- Saucey architecture that allows porting to new technologies with ease (from SDL2 to MonoGame in 3 hours!)
- Defies modern content pipelines by 
  - Reducing the hours in the development process (save $!), documented at 5 days and 2 artists down to X hours and 1 dev.
  - reducing the number of steps in the process of individual programs
  - Reducing the number of programs needed to work in (eventually the whole pipeline)
  - Non-Conventional design that empowers creators (innovation, yeah!)
  - Creating an environment designed from the ground up for collaboration and production while making it *fun*!
  - Makes work feel like play


## Rendering
- Monogame mvp, porting to vulkan (pipeline 75% done, using C# for faster iterations)
- Hot reloading shaders
- data driven network design for deterministic updates immediate upon receiving incoming data

## Architecture
- Data Oriented for runtime by design to sync over the network and application performance
- Rendering Queue: Batched Render Directed Acyclic Graph (DAG)
- Quad tree and map traversal to sync clients, teleport and manage a near-infinite graph for worlds
- Flexible UI framework agnostic to rendering
- Reference driven image processing
- Composite layering from ui framework to drawing layers
- GPU forwarding heavy graphics ops
- Shader-friendly system to offload procedural draw ops and high parallel ops

## Features
- UI
  - Child/Parent relationships
  - Real-time updates for user interactivity and flexibility
  - floating modal windows
  - Collapsing windows to save workspace when not in use.
  - Docking modals to actionbar for predictability and preference
  - Animated components
  - real-time with opt-in static to keep consistent visuals and allow for easy animations/shaders
  - UX designed to suit optimal workflows containing enough assumptions to prevent bad ones
  - Designed for *everyone* not just devs (as an artist and dev, artists get the shaft in game dev. devs left to clean up what they shouldn't have to)
- Draw canvas
  - Pixel art drawing
  - Layer Support
  - Keybindings for flow
  - Transformations on selection (rotate/flip)
  - Real-time editing of sprites across the world (edit one tile update the world)
- Color Swatch
  - RGB color picker with flair
  - Hue (box), Sat, Shad (sliders)

## Future Plans: Pixel Engine
- Scalability phase of UX, categories, containers, map markers to teleport to, ect.
- Animator/animations
- Domain Specific Language (programming language) for shaders with hot reload (already implemented!)
- Self-written compiled scripting language with hot reload (network synced changes)
- Languages that are easier to read/write (no, python could do better.)
- High performance scripting of shaders/game behaviors (yes, I'm looking at you python)
- Simple inline code blocks on top level object (like scratch blocks, but write code in them)
- Text file code for bigger systems with OOP built in (ready to scale!)
- Quick output to Pixi.js browser-native multiplayer project (better than competition)
- Port to Vulkan for more rendering control (render pipeline about 70-80% complete)
- Introducing flavors; *isometric*, *2d vector*, *voxel*, *3d*
- One editor version with project conversion (no, you don't have to tell someone 2025.2.3.4.1f.3x.33potato.8zab in the vc anymore)
- Isolated libraries that do not include bloat in your project with lightweight builds
- Landing app to connect the libraries and only provide what's necessary for your project with templates that do not bloat your games

## Future Plans: Platform
- Network resources for processing
- Data stored, encrypted and handled on server backend for security, quick build speeds and no more vpn nightmares
- KanBan, Canvas Collab, and Game-ified "quests" to track them in engine, and across projects
- User profiles for potential hiring/portfolios linking to work actually done
- Browser based Multiplayer game running for example of capability (project is done, no money to host server, digiverse.life) 
- Integrating all flavors (Pixel, Isometric, Vector, Voxel, 3d, hopefully a new medium?)
