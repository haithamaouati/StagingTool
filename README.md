# StagingTool
##### How to use Staging Tool to discover Windows 11’s secret features

The Staging Tool is apparently a software device used by Microsoft’s engineers to unlock features in Windows 11. It uses command lines to test the features, and it was spotted by [this Windows enthusiast](https://twitter.com/XenoPanther/status/1686712381840179200?s=20), in an apparent leak.

Of course, the post it was featured on is now deleted, but you can actually [download the Staging Tool from here]() and try it for yourself.

##### So how does Staging Tool work?

To properly use it, you need to have a bit of knowledge of using command-line tools, otherwise, you could end up breaking your system. However, the Windows enthusiast who discovered the tool also pushed it to reveal the commands that you can unlock.

Here are the command-lines you can use in Staging Tool:

* `/enable` – Enable the specified feature/disable – Disable the specified feature
* `/query` – Query the specified feature for enablement and viariant information.
* `/v` – optional parameter to also print ImageDefault and ImageOverride features
* `/reset` – Reset the specified feature to its default state
* `/testmode` – Used in conjunctions with /enable /disable /reset
* `/telemetry` – Used in conjuctions with /enable /disable /reset
* `/setvariant` – Select a feature variant to use; used in conjunction with `<featureId>` `<variantId>`
* `/serialize` – Use this option to print out a new config with all of the requested changes. This can be used for offline updates to VHDs prior to first boot.
* `/setlkg` – Set Boot time feature override states as LKG Configurations
* `/restorelkg` – Restore Boot time LKG configurations states Feature Configurations
* `/trace` – Realtime ETW trace for the specified feature usage in code.

To use them, you just have to add the keywords after StagingTool.exe in the terminal line as it follows:

```
StagingTool.exe [/enable <featureId>]
```
```
StagingTool.exe [/disable <featureId>]
```
```
StagingTool.exe [/query <featureId>]
```

If this seems complex to you, and you’re not a developer, then it’s better not to try it, as you can damage your Windows 11. On the other hand, for those of your who are familiar with it, you may now discover Windows 11’s hidden treasures. Of features.
