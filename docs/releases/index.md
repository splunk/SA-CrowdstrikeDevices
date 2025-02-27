---
order: -100
icon: project-roadmap
label: Releases
---

# Release Notes

Latest release can be found on [Splunkbase <small>:icon-link-external:</small>](https://splunkbase.splunk.com/app/6573){ target="blank" }.

## v1.1.5 [!badge text="LATEST" variant="info" icon="package"]

Released: [October 8, 2024 <small>:icon-link-external:</small>](https://github.com/splunk/SA-CrowdstrikeDevices/releases/tag/v1.1.5){ target="blank" }

+++ New :icon-shield-check:
- [x] Added CSV lookup for ES to use.
- [x] Added Serial Number to category field - feature request [#67](https://github.com/splunk/SA-CrowdstrikeDevices/issues/67){ target="blank" }
+++ Improved :icon-thumbsup:
- [x] Disabled KVstore replication to improve performance.
- [x] Increased batch size of KVstore lookup to improve performance. 
- [x] Removed type definition for KVstore fields. 
+++ 

Full Changelog: [v1.1.4...v1.1.5 <small>:icon-link-external:</small>](https://github.com/splunk/SA-CrowdstrikeDevices/compare/v1.1.4...v1.1.5){ target="blank" }

---

## v1.1.4

Released: [December 12, 2023 <small>:icon-link-external:</small>](https://github.com/splunk/SA-CrowdstrikeDevices/releases/tag/v1.1.4){ target="blank" }

+++ Fixed :icon-bug:
- [x] Fixed location of the "static" directory. Moved from the "default" directory to the project root. 

!!!important Note
This has no functional updates.
!!!
+++ 

Full Changelog: [v1.1.3...v1.1.4 <small>:icon-link-external:</small>](https://github.com/splunk/SA-CrowdstrikeDevices/compare/v1.1.3...v1.1.4){ target="blank" }

---

## v1.1.3

Released: [December 7, 2023 <small>:icon-link-external:</small>](https://github.com/splunk/SA-CrowdstrikeDevices/releases/tag/v1.1.3){ target="blank" }

+++ Improved :icon-thumbsup:
- [x] Added managed configurations for Splunk Enterprise Security to control retention of lookup file --> [Schedule Search](/start/scheduled-search.md){ target="blank" }
+++ Deprecated :icon-diff-removed:
- [x] Deprecating use of the search macro "sa_crowdstrike_retention" and the corresponding saved search.
+++

Full Changelog: [v1.1.2...v1.1.3 <small>:icon-link-external:</small>](https://github.com/splunk/SA-CrowdstrikeDevices/compare/v1.1.2...v1.1.3){ target="blank" }

---

## v1.1.2

Released: [December 1, 2023 <small>:icon-link-external:</small>](https://github.com/splunk/SA-CrowdstrikeDevices/releases/tag/v1.1.2){ target="blank" }

+++ New :icon-shield-check:
- [x] SplunkWorks updates

This release has no functional changes of the add-on.

---

## v1.1.1

Released: April 19, 2023

+++ New :icon-shield-check:
- [x] New format for the `category` field, see [Category](/components/category.md).
    - The `cs_` prefix has been removed from many fields.
    - Spaces have been added for easier readability.
+++ Fixed :icon-bug:
- [x] Hotfix for priority field failing default regex match
+++

---
 
## v1.0.5

Released: December 19, 2022

+++ New :icon-shield-check:
- [x] Added macro and retention definition to the General Settings in Splunk Enterprise Security
+++

---

## v1.0.4

Released: November 22, 2022

+++ New :icon-shield-check:
- [x] Added managed configuration to Splunk Enterprise Security
+++ Fixed :icon-bug:
- [x] Fixed incorrect mac field (Thanks [@PaddlingCode <small>:icon-link-external:</small>](https://github.com/PaddlingCode){ target="blank" })
+++

---

## v1.0.3 

Released: September 20, 2022

+++ New :icon-shield-check:
- [x] added cleanup search to remove old/stale devices
- [x] added search macro for device retention period
+++ Improved :icon-thumbsup:
- [x] updated collection to include last seen field
- [x] updated lookup generating search to include last time seen
+++

---

## v1.0.2

Released: September 8,2022

+++ New :icon-shield-check:
- [x] added `first_seen`, `last_seen`, and `last_updated` to category field
- added `site_name` to existing `bunit` field
+++ Improved :icon-thumbsup:
- [x] Changed app logo background to transparent.
- [x] Updated saved search to preserve hosts with multiple IP/MAC addresses
+++

---

## v1.0.1

Released: August 25, 2022

- [x] Hotfix for missing `_key` field in saved search.

---

## v1.0.0 

Released: August 25, 2022

- [x] Initial Release
