# All Configurations

Below is a table that list all configuration for this add-on.

Name | Type | Web Location | CLI Location\* | Description
---- | ---- | ------------ | ------------- | -----------
Crowdstrike Devices Lookup - Gen | Saved Search | Settings > Searches reports, and alerts | savedsearches.conf | Populates the lookup file `crowdstrike_devices`.
Crowdstrike Devices Lookup - Cleanup | Saved Search | Settings > Searches reports, and alerts | savedsearches.conf | removes old entries from kvstore lookup: `crowdstrike_devices`.
crowdstrike_devices | lookup | Settings > Lookups > Lookup definitions | transforms.conf | Lookup definition for the KVStore collection `crowdstrike_devices_collection`.
crowdstrike_devices_collection | KVStore collection | n/a\*\* | collections.conf | KVStore configuration.
sa_crowdstrike_index | Search macro | Settings > Advanced Search > Search Macros | macros.conf | Index definition for the crowdstrike index that contains the sourcetype `crowdstrike:device:json`.
sa_crowdstrike_retention | Search macro | Settings> Advanced Search > Search Macros | macros.conf | The amount of time for the device not being updated before it is removed from the lookup. `default "-2d"`
identity_manager://crowdstrike_devices | Asset lookup configuration | Enterprise Security > Configure > Data Enrichment > Asset and Identity Management > Asset Lookups | inputs.conf | Asset configuration lookup to load Crowdstrike devices into the asset database.

> \*CLI locations are relative to `../default`. Any update to CLI configuration files should be done in the local directory.

!!!info
**If you have the [Splunk App for Lookup File Editing<small>:icon-link-external:</small>](https://splunkbase.splunk.com/app/263){ target="blank" }, the KVStore collection `crowdstrike_devices_collection` is viewable within the Web interface.
!!!
