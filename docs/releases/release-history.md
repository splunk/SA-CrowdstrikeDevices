# Release history

## [v1.1.0 <small>March 26, 2023</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/releases/tag/v1.1.0)

### Compatibility

Product | Version
--------- | -------
Splunk platform versions | 9.x, 8.x
Splunk Enterprise Security version | [7.x, 6.x](https://splunkbase.splunk.com/app/263)
Crowdstrike Device Add-on Version | [3.x](https://splunkbase.splunk.com/app/5570)

### What's Changed

- New format for the `category` field:
    - The `cs_` prefix has been removed from many fields.
    - Spaces have been added for easier readability.

=== "New"

    ``` yaml
    bios: Dell Inc
    bios_version: 1.6.5
    cs_agent_version: 6.44.15806.0
    cs_dv_control_applied: true
    cs_dv_firewall_applied: true
    cs_dv_globalconfig_applied: true
    cs_dv_sensorupdate_applied: true
    cs_first_seen: 10/15/20 00:31:59 UTC
    cs_last_seen: 09/14/22 15:06:50 UTC
    cs_uninstallprotection: ENABLED
    dvc_manufacturer: Dell Inc
    dvc_name: OptiPlex 5050
    dvc_status: normal
    dvc_type: Workstation
    external_ip: 165.225.10.253
    gen: sa-crowdstrike
    os_major_version: 10
    os_name: Windows 10
    os_platform: Windows
    os_version: 10.0.19044.1889
    provision_status: Provisioned
    reduced_functionality_mode: no
    splunk_last_updated: 03/27/23 02:09:24 UTC
    ```

=== "Old"

    ``` yaml
    cs_agent_version:6.44.15806.0
    cs_bios_mf:dell_inc
    cs_bios_version:1.6.5
    cs_dv_control_applied:true
    cs_dv_firewall_applied:true
    cs_dv_globalconfig_applied:true
    cs_dv_sensorupdate_applied:true
    cs_dv_status:normal
    cs_dv_type:workstation
    cs_external_ip:165.225.10.253
    cs_os_major_version:10
    cs_os_name:windows_10
    cs_os_platform:windows
    cs_sys_mf:dell_inc
    cs_sys_name:optiplex_5050
    cs_uninstallprotection:enabled
    gen:sa_crowdstrike
    cs_first_seen:10/15/20 00:31:59 UTC
    cs_last_seen:09/14/22 15:06:50 UTC
    splunk_last_updated:03/27/23 02:14:24 UTC
    ```

**Full Changelog**: [v1.0.5...v1.1.0](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/compare/v1.0.5...v1.1.0)

## Known issues

Issue | Description | Solution | GitHub issue reference
----- | ----------- | -------- | ----------------------
Lookup file error | You may see the error `status="Lookup file error, unknown path or update time" name=crowdstrike_devices` | This error exists since the KVstore is being used opposed to a csv file and does not interfere with the functionality of lookup creation. | Issue [#22](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/22)

 Issues can be reported on the [SA-CrowdstrikeDevices's Github page](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues).
 
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
