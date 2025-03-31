# Getting started Modding Boxel 3D

Boxel 3D is a physics-based game built with **Three.js** for rendering and **Matter.js** for physics. Modding the game allows you to modify mechanics, add new features, or change visuals to create a custom experience.

## First Steps to Modding

### 1. Think of an Idea  
Before diving into code, decide what you want to change. Do you want to add a new movement type, or modify physics? Having a clear goal helps guide your modifications.

### 2. Learn JavaScript  
Since Boxel 3D is built using JavaScript, you need to understand its syntax and concepts, such as:  

- Variables, functions, and objects  
- Basic DOM manipulation  
- Understanding **Three.js** (for rendering) and **Matter.js** (for physics)  

### 3. Use a Code Editor  
To write and edit JavaScript code, use a text editor like:  

!!! tip "Recommended Code Editors"
    - **[Visual Studio Code](https://code.visualstudio.com/)** – A powerful editor with extensions and debugging tools.  
    - **[Notepad++](https://notepad-plus-plus.org/)** – A lightweight option with syntax highlighting.  

### 4. Access the Game Console  
Boxel 3D runs in a web browser, so you can use the built-in developer console to test changes.  

#### Steps to Open the Console:
1. Open the game in a browser.  
2. Look at the introduction page and see "Commands" for steps on how to open the console.
3. Navigate to the **Console** tab to enter JavaScript commands.  

Once you're comfortable with these basics, you can start modifying game elements by injecting custom scripts or editing local copies of the game files.  

🚀 **Next Steps:** Experiment with JavaScript commands in the console to manipulate game elements in real time!


# Event List

This part of the page includes lists of the events in Boxel 3D.

## Game Events

### General Events
| Event Name             | Detail Type  | Description |
|------------------------|-------------|-------------|
| `beforeSettingsClosed` | `{}`        | Triggered before settings are closed. |
| `closePopup`          | `{}`        | Fires when a popup is closed. |
| `levelStart`          | `{ detail: Object }` | Called when a level starts. |
| `levelFinished`       | `{ detail: Object }` | Triggered when a level is completed. |
| `openLevelSelectorPopup` | `{}`    | Fires when the level selector popup opens. |
| `openPopup`          | `{ detail: Object }` | Called when a popup is opened. |
| `pageMounted`        | `{ detail: String }` | Fired when a page is mounted. |
| `popupClosed`        | `{}`        | Triggered when a popup is closed. |
| `popupOpened`        | `{}`        | Fires when a popup is opened. |

### Player Events
| Event Name             | Detail Type  | Description |
|------------------------|-------------|-------------|
| `playerKill`         | `{ detail: { player: Object } }` | Triggered when a player is killed. |
| `playerRespawn`      | `{ detail: { player: Object } }` | Fires when a player respawns. |
| `playerRestart`      | `{ detail: { player: Object } }` | Called when a player restarts. |

### UI & Settings Events
| Event Name             | Detail Type  | Description |
|------------------------|-------------|-------------|
| `setCredit`          | `{ detail: { text: String } }` | Updates credit text. |
| `setMode`           | `{ detail: String }` | Sets the current game mode. |
| `setPage`           | `{ detail: String }` | Changes the current page. |
| `setSelectedObject` | `{ detail: Object }` | Sets the selected object in the UI. |
| `setSelectedMode`   | `{ detail: String }` | Changes the selected mode. |
| `setTheme`         | `{ detail: String }` | Sets the game theme. |
| `settingsClosed`    | `{}`        | Fires when the settings menu is closed. |
| `settingsOpened`    | `{}`        | Fires when the settings menu is opened. |
| `themeSelected`     | `{ detail: Object }` | Triggered when a theme is selected. |
| `updateLoading`     | `{ detail: Object }` | Updates the loading state. |
| `updateStatsVisibility` | `{}`    | Updates the visibility of stats. |

---

🚀 **Usage Example:**  
To listen for an event in Boxel 3D, use JavaScript like this:

## Simple respawn mod

    window.addEventListener("playerRespawn", (event) => {
        console.log("Player respawned:", event.detail.player);
    });

??? info inline "What does this do?"

    This mod listens to when the player respawns. If the player respawns, the console logs "Player respawned"
