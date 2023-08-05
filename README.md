# StagingTool
Microsoft Windows 11 StagingTool — Controls the feature configurations for this device.

![screenshot](https://raw.githubusercontent.com/haithamaouati/StagingTool/main/screenshot.jpg)

> Discovered by [XenoPantger](https://twitter.com/XenoPanther/status/1686712381840179200?s=20), in an apparent leak.

## Usage

Usage: `StagingTool.exe`


* `/enable` – Enable the specified feature
```
StagingTool.exe [/enable <featureId>]
```
* `/disable` – Disable the specified feature
```
StagingTool.exe [/disable <featureId>]
```
* `/query` – Query the specified feature for enablement and viariant information.
```
StagingTool.exe [/query <featureId>]
```
* `/v` – optional parameter to also print ImageDefault and ImageOverride features
* `/reset` – Reset the specified feature to its default state
* `/testmode` – Used in conjunctions with /enable /disable /reset
* `/telemetry` – Used in conjuctions with /enable /disable /reset
* `/setvariant` – Select a feature variant to use; used in conjunction with `<featureId>` `<variantId>`
* `/serialize` – Use this option to print out a new config with all of the requested changes. This can be used for offline updates to VHDs prior to first boot.
* `/setlkg` – Set Boot time feature override states as LKG Configurations
* `/restorelkg` – Restore Boot time LKG configurations states Feature Configurations
* `/trace` – Realtime ETW trace for the specified feature usage in code.

## Feature IDs
[Mach2 feature IDs](https://github.com/riverar/mach2/tree/master/features)

## Disclaimer
> We are not responsible for any misuse or damage caused by this program. use this tool at your own risk!
> 
