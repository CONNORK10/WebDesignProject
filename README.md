# Adventure Game Design and Tech Spec

---

## 1. Project Choice
- **Option:** Web Game Design  
- **Game Title:** “Tree of Realms”

---

## 2. Purpose of the Game

### Goal
The main purpose of *Tree of Realms* is to provide players with an immersive, progressive adventure where they climb the "World Tree," inspired by Norse mythology’s Yggdrasil. Players explore various biomes, each a distinct world or "realm" along the tree’s branches, each leading to unique challenges, resources, and bosses. The ultimate objective is to reach the top and defeat a powerful final boss to achieve glory and complete the game.

### Target Audience
- **Age Group:** 8 and up  
- **Interests:** Adventure gaming enthusiasts, fantasy fans, young gamers interested in open-world exploration, and fans of mythology.  
- **User Needs:** An engaging, easy-to-navigate game that encourages exploration and problem-solving while offering challenging encounters for players of various ages.

---

## 3. Design

### A. Functionality

#### Core Features
- **Tree Climbing and Navigation:** Players move their character up through levels of the World Tree, each level representing a unique biome.  
  - **Controls:** 
    - **Arrow Keys:**  
      - **Up Arrow:** Jump  
      - **Left Arrow:** Move Left  
      - **Right Arrow:** Move Right  
    - **E Key:** Opens inventory
    - **Spacebar:** Interact with NPCs or objects
    - **Shift Key:** Run or sprint
- **Procedurally Generated Map:** Each biome is procedurally generated, making every exploration unique and encouraging players to find secrets and hidden areas.
- **Resource Collection and Inventory System:** Resources such as herbs, minerals, and magical items can be gathered to aid the player.
  - **Bag Storage:** Players have an inventory bag for storing collected items, which can be upgraded as they progress to carry more items. Players can choose to use items for immediate benefits or collect them for crafting or trading.
- **Biome Diversity and Progression:** Each biome has a unique boss that must be defeated to advance to the next level of the tree. Each boss drops valuable loot that helps the player prepare for future challenges.
- **NPC Interactions and Villages:** Friendly NPCs inhabit small villages within each biome. Some offer helpful services, like crafting or forging better items, while others may act as traders or give quests. There are also hostile NPCs and mobs that increase the level of danger in each area.

#### User Flow
1. **Start Screen:**  
   - **Options:** New Game, Continue, Instructions, and Settings.
   - **Instructions:** Overview of movement, resource gathering, NPC interaction, and combat mechanics.
2. **Gameplay:**  
   - **Initial Spawn:** Player appears in the first biome of the World Tree with a brief tutorial on the basics.
   - **Objective:** Progress through each level of the tree by defeating bosses, interacting with NPCs, gathering resources, and upgrading items.
3. **Level Progression:**  
   - **Biome Unlocks:** Defeating the boss of each biome allows the player to ascend to the next biome level on the tree.
4. **Game Over Screen:**  
   - Final achievements and glory score display, with options to replay or return to the start screen.

#### Mechanics
- **Movement:** Player can walk, run, jump, and climb using a combination of arrow keys and the shift key.
- **Resource Collection and Inventory Management:** Resources are collected by interacting with specific objects and NPCs, then stored in the player’s bag.
- **Combat and Boss Fights:** Each biome has mobs and a unique boss that must be defeated to progress. Bosses drop rare loot, with each biome boss becoming progressively more challenging.
- **NPC Interactions:** Players can converse, trade, or accept quests from friendly NPCs in villages scattered across the biomes.

#### Interactive Elements
- **Buttons:** Start, Pause, Map, Inventory, and Quest Log buttons accessible during gameplay.
- **HUD (Heads-Up Display):**  
  - **Health Bar:** Displays player’s health level.
  - **Inventory Bag:** Shows the items collected and bag storage level.
  - **Quest Log:** Displays active objectives and quest hints.
  - **Biome Indicator:** Shows the current biome name and the level of the tree.

---

### B. Aesthetics

#### Visual Style
- **Theme:** Mythical, adventure-inspired style that merges natural and fantasy elements to create unique, atmospheric biomes along the tree.
- **Imagery and Iconography:**  
  - **Environment:** Each biome on the tree features different settings such as mystical forests, desert landscapes, frozen tundras, and volcanic realms.
  - **Characters and NPCs:** Semi-cartoonish yet detailed characters for broad appeal, including villagers, merchants, and mythical creatures.
  - **Icons:** Distinct symbols for items, resources, and actions to help younger players quickly identify their use and function.

#### Color Scheme
- **Palette:** Earthy and mystical tones, with greens and browns for the base of the tree, and color variations to distinguish each biome (e.g., icy blues for snow areas, warm reds for volcanic areas).
- **Color Psychology:** Colors designed to encourage exploration, excitement, and a sense of adventure.

#### Typography
- **Font Style:** Bold, fantasy-style fonts for immersive feel, with clear readability for younger players on the HUD elements.

#### Layout
- **Screen Arrangement:**  
  - **Game Area:** Biomes occupy the majority of the screen, providing a scenic view of each level.
  - **HUD Elements:** Inventory, health, and quest indicators are positioned in corners for easy access.
  - **Navigation:** Start screen, map view, and inventory screen for smooth game flow.

---

## Technical Specifications

### 1. Technology Stack
- **Programming Language:** JavaScript, with WebGL for advanced graphical effects
- **Game Framework:** Phaser.js or Babylon.js for robust 2D/3D game support
- **Frontend:** HTML5 and CSS3 for UI

### 2. Architecture
- **MVC Pattern:** Separates game logic, UI, and data, enabling modular updates and improved performance.

### 3. Data Model
- **Biomes and Tree Levels:** Each biome is represented as a node on the tree, with properties defining resources, hazards, NPCs, and specific boss traits.
- **Characters:** Objects with properties for position, direction, health, and inventory.
- **Resources and Items:** Items stored in a procedurally generated inventory, with each biome yielding unique resources and crafting materials.

### 4. Security and Performance
- **Client-Side Rendering:** Game runs in the user’s browser, optimized for low latency and smooth transitions.
- **Optimized Graphics:** Lightweight assets and procedurally generated maps for faster load times and varied experiences.

---

### 5. Specific Functionalities

**a. Movement and Collision Detection**  
- **Specification:** Phaser’s physics engine provides responsive control over jumping, climbing, and navigating obstacles, ensuring smooth control response.

**b. Resource Collection and Inventory Management**  
- **Specification:** Track items collected and store them in a progressively upgradable inventory bag system. Items can be used for crafting or stored for trade.

**c. Procedurally Generated Biomes and Boss Battles**  
- **Specification:** Each biome is procedurally generated, with distinct themes and bosses that provide high-level loot. Bosses at each level increase in difficulty.

**d. NPC Interactions and Villages**  
- **Specification:** NPCs offer quests, crafting services, and trade. Villages are populated with friendly NPCs, with enemy NPCs adding an element of danger.

**e. Sound Effects and Background Music**  
- **Specification:** Phaser’s audio manager delivers ambient sounds and effects tailored to each biome, enhancing immersion and depth.

**f. User Interface and Responsiveness**  
- **Specification:** HTML5 and CSS3 for responsive UI across devices, optimized for desktops and tablets.

---

This design builds an immersive experience where players journey through a mythological World Tree, ascending through biomes, encountering unique challenges, and ultimately reaching a climactic boss fight at the top.