---
order: -100
icon: project-roadmap
label: Releases
---

# Release Notes

Latest release can be found on [Splunkbase <small>:icon-link-external:</small>](https://splunkbase.splunk.com/app/6573){ target="blank" }.

## v1.1.1 [!badge text="LATEST" variant="info"]

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
