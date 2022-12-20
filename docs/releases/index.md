# Release notes

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

## Known issues

Issue | Description | Solution | GitHub issue reference
----- | ----------- | -------- | ----------------------
Lookup file error | You may see the error `status="Lookup file error, unknown path or update time" name=sa_aws_assets` | This error exists since the KVstore is being used opposed to a csv file and does not interfere with the functionality of lookup creation. | Issue [#22](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/22)

 Issues can be reported on the [SA-CrowdstrikeDevices's Github page](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues).
