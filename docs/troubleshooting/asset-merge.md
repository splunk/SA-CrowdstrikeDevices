# Asset Merge

 It is possible that some of your devices share a common key field (`dns`, `ip`, `mac`, `nt_host`) that is causing an erroneous merge of your assets. There are a few ways to overcome this:

- [Asset Merge](#asset-merge)
  - [Problem Scenario](#problem-scenario)
    - [Default merge](#default-merge)
    - [Expected behavior](#expected-behavior)
  - [Solutions](#solutions)
    - [Disable Asset Merging](#disable-asset-merging)
    - [Update Asset Key Fields](#update-asset-key-fields)

## Problem Scenario

Consider you have the following assets:

Host | dns | ip | mac | nt_host
---- | --- | -- | --- | -------
host1 | host1.local | ==10.0.34.9== | 77:61:f5:cb:33:a7 | host1
host2 | host2.local | ==10.0.34.9== | a5:e7:5c:39:77:d1 | host2

Since these two systems share the same IP they will be merged into a single asset by default.

### Default merge

Asset | dns | ip | mac | nt_host
----- | --- | -- | --- | -------
host1<br>host2<br>host1.local<br>10.0.34.9<br>77:61:f5:cb:33:a7<br>a5:e7:5c:39:77:d1 | host1.local<br>host2.local | 10.0.34.9 | 77:61:f5:cb:33:a7<br>a5:e7:5c:39:77:d1 | host1<br>host2

### Expected behavior

<small>_see next section to accomplish this expected behavior_</small>

Asset | dns | ip | mac | nt_host
----- | --- | -- | --- | -------
host1<br>host1.local<br>10.0.34.9<br>77:61:f5:cb:33:a7 | host1.local | 10.0.34.9 | 77:61:f5:cb:33:a7 | host1
host2<br>host2.local<br>10.0.34.9<br>a5:e7:5c:39:77:d1 | host2.local | 10.0.34.9 | a5:e7:5c:39:77:d1 | host2

## Solutions

### Disable Asset Merging

If Crowdstrike is your **_only_** data source for assets, you can disable asset merge in the global settings.

!!!warning This is not recommended if you have more than one asset list configured (see next section)
!!!

1. In Enterprise Security navigate to Configure > Data Enrichment > Asset and Identity Management > Global Settings.
2. Toggle off "Assets" under `Enable Merge for Assets or Identities`.

Changes should reflect the next time the Asset database builds (usually 5-10 minutes).

<small>\*_For more information, see [Splunk Docs:icon-link-external:](https://docs.splunk.com/Documentation/ES/latest/Admin/Merge){ target="blank" }._</small>

### Update Asset Key Fields

If you have more than one asset list configured you can look at disabling the common key field to prevent the default merging behavior.

!!!success In most cases, the IP field will be field that needs to disabled as the key field.
!!!

1. (In Enterprise Security) Navigate to Configure > Data Enrichment > Asset and Identity Management.
1. Select the "Asset Fields" Tab.
1. Select the `ip` field (or the field you want to disable) and "uncheck" it from being a Key.

![Disable Asset Key by unchecking "Key"](/static/asset-key-field.png)

Changes should reflect the next time the Asset database builds (usually 5-10 minutes).
