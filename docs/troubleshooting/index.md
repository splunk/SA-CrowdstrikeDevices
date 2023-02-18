# Troubleshooting

There can be many issues when setting up a new app/add-on in Splunk. Below highlights the most common issues with this Add-on. Don't see your issue? Submit a new issue on [Github](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues).

Issue | Description | Solution
----- | ----------- | --------
Multiple asset merge | It is possible that some of your devices share a common key field (`dns`, `ip`, `mac`, `nt_host`) which will cause merging by default. |See the [Asset Merge Solutions](./solution-guides/asset-merge) for ways to improve the merging behavior.
Asset Database not populating with Crowdstrike Data | The asset database may show no Crowdstrike data if the initial search has not run to build the asset database or the default macro has not been updated. | Verify the default macro has the correct index definition (see [Update Default Macro](/quickstart/quickstart/#update-default-macro)). Also see [Force build](/quickstart/quickstart/#force-initial-build) to build the Crowdstrike assets lookup before the first scheduled run.
