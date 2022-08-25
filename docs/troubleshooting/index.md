# Troubleshooting

There can be many issues when setting up a new app/add-on in Splunk. Below highlights the most common issues with this Add-on. Don't see your issue? Submit a new issue on [Github](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues).

Issue | Description | Solution
----- | ----------- | --------
Multiple asset merge | It is possible that some of your devices share a common mac address or another key field which will cause merging by default. | If Crowdstrike is your only asset source you can disable asset merge under global settings. See [Asset Merge Solution](./solution-guides/asset-merge) for more information.
