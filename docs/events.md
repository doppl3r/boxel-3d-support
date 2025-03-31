# Event List

This part of the page includes lists of the events in Boxel 3D.

## Game Events

### 1. General Events
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

### 2. Player Events
| Event Name             | Detail Type  | Description |
|------------------------|-------------|-------------|
| `playerKill`         | `{ detail: { player: Object } }` | Triggered when a player is killed. |
| `playerRespawn`      | `{ detail: { player: Object } }` | Fires when a player respawns. |
| `playerRestart`      | `{ detail: { player: Object } }` | Called when a player restarts. |

### 3. UI & Settings Events
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
