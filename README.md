# Home Assistant Room Presence Combiner Blueprint

This blueprint combines multiple presence sensors into a single virtual room presence sensor. If any sensor detects presence, the room is set to "occupied." When all sensors are inactive, the room is set to "unoccupied." You can also define custom states or thresholds for each sensor directly from the blueprint configuration page.

[![Open your Home Assistant instance and show the blueprint import dialog with this blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?url=https://github.com/ukit-network/home-assistant-room-presence-blueprint/blob/main/room_presence_combiner_configurable.yaml)

---

## Features
- Combine multiple presence sensors into one virtual room sensor.
- Support for custom states/thresholds for each sensor.
- Easy configuration via the Home Assistant UI.

---

## Installation

1. **Click the button above** to import the blueprint directly into your Home Assistant setup.
2. Place the YAML file manually if needed:
   - Save the file as `room_presence_combiner_configurable.yaml` in the `blueprints/automation/` directory of your Home Assistant configuration.
   - Reload Automations in Home Assistant.

---

## Usage

1. Navigate to **Settings > Automations & Scenes > Blueprints > Import Blueprint**.
2. Use this blueprint to configure:
   - **Presence Sensors:** Select the sensors to monitor for presence.
   - **Sensor Conditions:** Specify the states or thresholds that indicate presence.
   - **Virtual Sensor:** Select an `input_boolean` helper to act as the room's presence indicator.

### Example:
- Sensors:
  - `binary_sensor.living_room_motion` (State: `on`)
  - `binary_sensor.door_sensor` (State: `open`)
  - `sensor.light_sensor` (Threshold: `> 30`)

---

## Contributions
Feel free to open issues or submit pull requests for improvements or bug fixes!

---

## License
This project is licensed under the MIT License.