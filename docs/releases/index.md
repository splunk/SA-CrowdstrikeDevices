# Release notes

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

## Known issues

Issue | Description | Solution | GitHub issue reference
----- | ----------- | -------- | ----------------------
Lookup file error | You may see the error `status="Lookup file error, unknown path or update time" name=sa_aws_assets` | This error exists since the KVstore is being used opposed to a csv file and does not interfere with the functionality of lookup creation. | Issue [#22](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/22)

 Issues can be reported on the [SA-CrowdstrikeDevices's Github page](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues).
