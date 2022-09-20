# Release history

## v1.0.2 <small>September 8,2022</small>

### Compatibility

Product | Version
--------- | -------
Splunk platform versions | 9.x, 8.x
Splunk Enterprise Security version | [7.x, 6.x](https://splunkbase.splunk.com/app/263)
Crowdstrike Device Add-on Version | [3.x](https://splunkbase.splunk.com/app/5570)

### New

- added `first_seen`, `last_seen`, and `last_updated` to category field ([#8](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/8)).
- added `site_name` to existing `bunit` field ([#13](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/13)).

### Updated

- Changed app logo background to transparent.

### Fixed

- Updated saved search to preserve hosts with multiple IP/MAC addresses ([#11](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/11)).

## v1.0.1 <small>August 25, 2022</small>

- Hotfix for missing `_key` field in saved search.

## v1.0.0 <small>August 25, 2022</small>

- Initial Release
