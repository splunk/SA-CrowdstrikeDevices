---
order: -100
icon: project-roadmap
label: Releases
---

# Release Notes

Latest release can be found on [Splunkbase<small>:icon-link-external:</small>](https://splunkbase.splunk.com/app/6573){ target="blank" } or [GitHub<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/releases/tag/v1.1.1){ target="blank" }.

## v1.1.1 [!badge text="LATEST" variant="info"]

Released: [April 19, 2023<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/releases/tag/v1.1.1){ target="blank" }

+++ New :icon-shield-check:
- [x] New format for the `category` field, see [Category](/components/category.md).
    - The `cs_` prefix has been removed from many fields.
    - Spaces have been added for easier readability.
+++ Fixed :icon-bug:
- [x] Hotfix for priority field failing default regex match - [#58<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/58){ target=blank }
+++

**Full Changelog**: [v1.0.5...v1.1.1<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/compare/v1.0.5...v1.1.1){ target="blank" }

---
 
## v1.0.5

Released: [December 19, 2022<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/releases/tag/v1.0.5){ target="blank" }

+++ New :icon-shield-check:
- [x] Added macro and retention definition to ES General Settings in [#35<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/commit/8a1f138b2a244e6b6bbc7cd07d6a4db7a2f67ab5){ target="blank" }
+++

**Full Changelog**: [v1.0.4...v1.0.5<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/compare/v1.0.4...v1.0.5){ target="blank" }

---

## v1.0.4

Released: [November 22, 2022<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/releases/tag/v1.0.4){ target="blank" }

+++ New :icon-shield-check:
- [x] Added ES managed configuration
+++ Fixed :icon-bug:
- [x] Fixed incorrect mac field (Thanks [@PaddlingCode<small>:icon-link-external:</small>](https://github.com/PaddlingCode){ target="blank" }) - [#30<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/30){ target="blank" }
+++

**Full Changelog**: [v1.0.3...v1.0.4<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/compare/v1.0.3...v1.0.4){ target="blank" }

---

## v1.0.3 

Released: [September 20, 2022<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/releases/tag/v1.0.3){ target="blank" }

+++ New :icon-shield-check:
- [x] added cleanup search to remove old/stale devices ([#18<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/18){ target="blank" }).
- [x] added search macro for device retention period ([#18<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/18){ target="blank" }).
+++ Improved :icon-thumbsup:
- [x] updated collection to include last seen field ([#18<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/18){ target="blank" }).
- [x] updated lookup generating search to include last time seen ([#18<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/18){ target="blank" }).
+++

---

## v1.0.2

Released: September 8,2022

+++ New :icon-shield-check:
- [x] added `first_seen`, `last_seen`, and `last_updated` to category field ([#8<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/8){ target="blank" }).
- added `site_name` to existing `bunit` field ([#13<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/13){ target="blank" }).
+++ Improved :icon-thumbsup:
- [x] Changed app logo background to transparent.
- [x] Updated saved search to preserve hosts with multiple IP/MAC addresses ([#11<small>:icon-link-external:</small>](https://github.com/ZachChristensen28/SA-CrowdstrikeDevices/issues/11){ target="blank" }).
+++

---

## v1.0.1

Released: August 25, 2022

- [x] Hotfix for missing `_key` field in saved search.

---

## v1.0.0 

Released: August 25, 2022

- [x] Initial Release
