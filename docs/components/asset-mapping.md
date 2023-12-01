# Asset Database Mapping

The following table describes how this add-on maps to the Asset Database.

> reference [Format an asset or identity in Splunk Enterprise Security <small>:icon-link-external:</small>](https://docs.splunk.com/Documentation/ES/latest/Admin/Formatassetoridentitylist#Asset_lookup_header){ target="blank" }

Asset lookup field | [CrowdStrike Device TA Fields <small>:icon-link-external:</small>](https://splunkbase.splunk.com/app/5570){ target="blank" } | Example value | Multi-value allowed
--- | --- | --- | ---
ip | `falcon_device.local_ip` | 10.15.23.8 | true
mac | `mac` | 61:se:e3:1s:7r:38 | true
nt_host | `falcon_device.hostname` | dev-server01 | false
dns | `nt_host` + `falcon_device.machine_domain` | dev-server01.example.com | true
owner | n/a | `not mapped` | n/a
priority | see [Configure Priority](/configure/priority.md) | medium | false
lat | from `iplocation` of `falcon_device.external_ip` | 40.76073 | false
long | from `iplocation` of `falcon_device.external_ip` | -111.89096 | false
city | from `iplocation` of `falcon_device.external_ip` | Salt Lake City | false
country | from `iplocation` of `falcon_device.external_ip` | United States | false
bunit | `falcon_device.ou{}` + `falcon_device.site_name` | computer,finance | true
category | see [Category field reference](category.md) | see [Category field reference](category.md) | true
pci_domain | n/a | `not mapped` | n/a
is_expected | n/a | `not mapped` | n/a
should_timesync | n/a | `not mapped` | n/a
should_update | n/a | `not mapped` | n/a
requires_av | n/a | `not mapped` | n/a
cim_entity_zone | n/a | `not mapped` | n/a
