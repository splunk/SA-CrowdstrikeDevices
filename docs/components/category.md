# Category Field

## Default category field mapping

Mapped Field | CrowdStrike Event Field | Example value
------------ | ----------------------- | -------------
bios | `falcon_device.bios_manufacturer` | Dell Inc
bios_version | `falcon_device.bios_version` | 1.6.5
cs_agent_version | `falcon_device.agent_version` | 6.40.15406.0
cs_dv_control_applied | `falcon_device.device_policies.device_control.applied` | true
cs_dv_firewall_applied | `falcon_device.device_policies.firewall.applied` | true
cs_dv_globalconfig_applied | `falcon_device.device_policies.global_config.applied` | true
cs_dv_sensorupdate_applied | `falcon_device.device_policies.sensor_update.applied` | true
cs_uninstallprotection | `falcon_device.device_policies.sensor_update.uninstall_protection` | enabled
cs_tags | `falcon_device.tags{}` | n/a
cs_first_seen | `falcon_device.first_seen` | 02/14/22 09:52:05 MST
cs_last_seen | `falcon_device.first_seen` | 08/24/22 13:25:24 MDT
os_major_version | `falcon_device.major_version` | 10
kernel_version | `falcon_device.kernel_version` | 10.0.19044.1889
os_platform | `falcon_device.platform_name` | windows
os_name | `falcon_device.os_version` | windows 10
dvc_type | `falcon_device.product_type_desc` | workstation
dvc_status | `falcon_device.status` | normal
dvc_manufacturer | `falcon_device.system_manufacturer` | hp
dvc_name | `falcon_device.system_product_name` | hp_elitebook_850_g7_notebook_pc
external_ip | `falcon_device.external_ip` | 0.0.0.0
reduced_functionality_mode | `falcon_device.reduced_functionality_mode` | no
splunk_last_update | n/a | 08/26/22 18:54:42 MDT

### Full example of category value

```yaml
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
