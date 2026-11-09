# Desk Lamp Computational Model

An interactive appliance model for a Doodle assignment on states, variables, control flow, and events.

## Run

Download `index.html` and open it in a modern web browser. The HTML, CSS, and JavaScript are in one self-contained file. No installation or external dependencies are required.

## Controls

- Click **Turn on** or **Turn off** to switch the lamp's power.
- Move the brightness slider between **1 and 100**.
- Select **Warm** or **Cool** light.
- Adjustment controls are disabled while the lamp is off.
- Turning the lamp off and on preserves its settings during the current page session. Reloading resets the model to off, brightness 70, and warm light.

## Computational model

| Variable | Initial value | Purpose |
| --- | --- | --- |
| `isOn` | `false` | Tracks the power state |
| `brightness` | `70` | Tracks brightness from 1 to 100 |
| `lightMode` | `"warm"` | Tracks warm or cool light |

User events (`click`, `input`, and `change`) update these variables and call `updateLamp()`. The function uses `if / else` to update the glow, status text, and controls.

## AI assistance

ChatGPT assisted with planning, the initial implementation, code comments, and state-logic checks. Browser rendering and manual user testing should be verified separately.
