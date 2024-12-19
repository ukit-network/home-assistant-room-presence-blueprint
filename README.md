# Home Assistant Room Presence Combiner Blueprint

This blueprint combines multiple presence sensors into a single virtual room presence sensor. If any sensor detects presence, the room is set to "occupied." When all sensors are inactive, the room is set to "unoccupied."

## Features
- Combine multiple sensors of different types.
- Support for custom states/values for each sensor.
- Flexible and easy to use.

## Installation
1. Clone this repository or download the `room_presence_combiner.yaml` file.
2. Place the blueprint file in your Home Assistant `blueprints/automation/` directory.
3. Reload the Automations in Home Assistant.

## Usage
1. Navigate to `Settings > Automations & Scenes > Blueprints > Import Blueprint`.
2. Select the `Room Presence Combiner` blueprint.
3. Configure the following:
   - Presence sensors and their corresponding states/values.
   - A virtual input_boolean sensor to represent the room's state.

## Example Use Case
- Motion sensors (`on` state).
- Door sensors (`open` state).
- Light sensors (threshold values).

## Contributions
Feel free to submit pull requests or create issues for enhancements or bug fixes!

## License
This project is licensed under the MIT License.
