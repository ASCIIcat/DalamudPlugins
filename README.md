# ASCIIcat's Dalamud Plugins

A shared custom repository for Dalamud plugins by AdelaideTheBun ♥.

## Installation

Once the repositories and release are published, add this URL in Dalamud Settings → Experimental → Custom Plugin Repositories, enable it, and save:

```text
https://raw.githubusercontent.com/ASCIIcat/DalamudPlugins/main/pluginmaster.json
```

Then install the desired plugin from the plugin installer.

## Plugins

- [Private Marks](https://github.com/ASCIIcat/PrivateMarks): private visual player marks and off-screen indicators.

## First publication

The initial Private Marks entry has `IsHide: true` until its download is available.

1. Publish the PrivateMarks source repository to ASCIIcat/PrivateMarks.
2. Create release v1.0.0 there and attach the generated PrivateMarks/bin/Release/PrivateMarks/latest.zip.
3. Confirm that the ZIP's manifest reports InternalName PrivateMarks, AssemblyVersion 1.0.0.0, and DalamudApiLevel 15.
4. Publish this repository to ASCIIcat/DalamudPlugins and verify the raw icon and catalogue URLs.
5. Verify the release download URL, set IsHide to false, and commit and push the catalogue change.
6. Test installation through the shared repository URL.

## Updating and adding plugins

Each plugin has its own source repository and versioned release ZIP. This repository contains only the shared catalogue and installer icons.

For an update, publish the new ZIP first, then copy the generated manifest version and API level into the matching catalogue entry and update both download URLs. Use versioned release links so the catalogue and archive stay in sync.

For another plugin, append another object to the JSON array with its unique InternalName, metadata, release links and icon. Keep Author exactly `AdelaideTheBun ♥` for our plugins and preserve third-party attribution.
