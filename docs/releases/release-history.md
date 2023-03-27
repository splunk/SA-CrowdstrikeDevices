# Release history

## [v1.0.5 <small>December 19, 2022</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/releases/tag/v1.0.5)

### Compatibility

Product | Version
--------- | -------
Splunk platform versions | 9.x, 8.x
Splunk Enterprise Security version | [7.x, 6.x](https://splunkbase.splunk.com/app/263)
Crowdstrike Device Add-on Version | [3.x](https://splunkbase.splunk.com/app/5570)

### What's Changed

- Added macro and retention definition to ES General Settings in [#35](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/commit/8a1f138b2a244e6b6bbc7cd07d6a4db7a2f67ab5)

**Full Changelog**: [v1.0.4...v1.0.5](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/compare/v1.0.4...v1.0.5)

### Known issues

Issue | Description | Solution | GitHub issue reference
----- | ----------- | -------- | ----------------------
Lookup file error | You may see the error `status="Lookup file error, unknown path or update time" name=crowdstrike_devices` | This error exists since the KVstore is being used opposed to a csv file and does not interfere with the functionality of lookup creation. | Issue [#22](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/22)

## [v1.0.4 <small>November 22, 2022</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/releases/tag/v1.0.4)

### Compatibility

Product | Version
--------- | -------
Splunk platform versions | 9.x, 8.x
Splunk Enterprise Security version | [7.x, 6.x](https://splunkbase.splunk.com/app/263)
Crowdstrike Device Add-on Version | [3.x](https://splunkbase.splunk.com/app/5570)

### What's Changed

- Added ES managed configuration
- Fixed incorrect mac field (Thanks [@PaddlingCode](https://github.com/PaddlingCode)) - [#30](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/30)

**Full Changelog**: [v1.0.3...v1.0.4](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/compare/v1.0.3...v1.0.4)

## [v1.0.3 <small>September 20, 2022</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/releases/tag/v1.0.3)

### Compatibility

Product | Version
--------- | -------
Splunk platform versions | 9.x, 8.x
Splunk Enterprise Security version | [7.x, 6.x](https://splunkbase.splunk.com/app/263)
Crowdstrike Device Add-on Version | [3.x](https://splunkbase.splunk.com/app/5570)

### What's Changed

- added cleanup search to remove old/stale devices ([#18](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/18)).
- added search macro for device retention period ([#18](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/18)).
- updated collection to include last seen field ([#18](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/18)).
- updated lookup generating search to include last time seen ([#18](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/18)).

## v1.0.2 <small>September 8,2022</small>

### Compatibility

Product | Version
--------- | -------
Splunk platform versions | 9.x, 8.x
Splunk Enterprise Security version | [7.x, 6.x](https://splunkbase.splunk.com/app/263)
Crowdstrike Device Add-on Version | [3.x](https://splunkbase.splunk.com/app/5570)

### What's Changed

- added `first_seen`, `last_seen`, and `last_updated` to category field ([#8](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/8)).
- added `site_name` to existing `bunit` field ([#13](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/13)).
- Changed app logo background to transparent.
- Updated saved search to preserve hosts with multiple IP/MAC addresses ([#11](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/11)).

## v1.0.1 <small>August 25, 2022</small>

- Hotfix for missing `_key` field in saved search.

## v1.0.0 <small>August 25, 2022</small>

- Initial Release
