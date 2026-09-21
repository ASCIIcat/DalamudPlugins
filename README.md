# ASCIIcat's Dalamud Plugins

A shared custom repository for Dalamud plugins by AdelaideTheBun ♥.

## Installation

Add this URL in Dalamud Settings → Experimental → Custom Plugin Repositories, enable it, and save:

```text
https://raw.githubusercontent.com/ASCIIcat/DalamudPlugins/main/pluginmaster.json
```

Then install the desired plugin from the plugin installer.

## Plugins

- [Private Marks](https://github.com/ASCIIcat/PrivateMarks): private visual player marks and off-screen indicators.

## Current release

Private Marks 1.0.1 is published and enabled. Its package manifest includes the hosted installer icon.

## Updating and adding plugins

Each plugin has its own source repository and versioned release ZIP. This repository contains only the shared catalogue and installer icons.

For an update, publish the new ZIP first, then copy the generated manifest version and API level into the matching catalogue entry and update both download URLs. Use versioned release links so the catalogue and archive stay in sync.

For another plugin, append another object to the JSON array with its unique InternalName, metadata, release links and icon. Keep Author exactly `AdelaideTheBun ♥` for our plugins and preserve third-party attribution.
