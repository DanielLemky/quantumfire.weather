# Weather

An Omalaunch extension for the weather tools included with Omarchy.

## Features

- Show the current Omarchy weather status.
- Open the detailed Omarchy weather panel.
- Set the weather location.
- Clear the saved location and return to automatic IP-based detection.

The extension uses the existing `omarchy-weather-status`, `omarchy-weather-location`, and `omarchy-notification-weather` commands. Weather data and location state remain owned by Omarchy.

## Requirements

- A current Omarchy installation with the `omarchy.weather` plugin enabled
- Omalaunch
- `jq`
- `timeout`

The extension does not install dependencies. It runs without elevated privileges. Omarchy owns the weather network requests and stores the selected location in its normal user state directory.

## Installation

Install and enable the plugin from GitHub:

```bash
omarchy plugin add https://github.com/DanielLemky/quantumfire.weather --enable
```

## Usage

1. Open Omalaunch.
2. Open **Extensions**.
3. Select **Weather**.
4. Select the current status to open the detailed forecast.
5. Press `Ctrl+K` on the status to set or clear the weather location.

You can star the Weather extension with `Ctrl+S` to put it on the Omalaunch starting view.

## Removal

Remove the plugin with Omarchy:

```bash
omarchy plugin remove quantumfire.weather
```

## License

MIT
