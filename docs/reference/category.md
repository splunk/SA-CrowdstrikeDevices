# Categories

## Default category field mapping

Mapped Field | Crowdstrike Event Field | Example value
------------ | ----------------------- | -------------
cs_agent_version | `falcon_device.agent_version` | 6.40.15406.0
cs_bios_mf | `falcon_device.bios_manufacturer` | hp
cs_bios_version | `falcon_device.bios_version` | s73_ver_01.08.00
cs_dv_control_applied | `falcon_device.device_policies.device_control.applied` | true
cs_dv_firewall_applied | `falcon_device.device_policies.firewall.applied` | true
cs_dv_globalconfig_applied | `falcon_device.device_policies.global_config.applied` | true
cs_dv_sensorupdate_applied | `falcon_device.device_policies.sensor_update.applied` | true
cs_uninstallprotection | `falcon_device.device_policies.sensor_update.uninstall_protection` | enabled
cs_os_major_version | `falcon_device.major_version` | 10
cs_os_platform | `falcon_device.platform_name` | windows
cs_os_name | `falcon_device.os_version` | windows_10
cs_dv_type | `falcon_device.product_type_desc` | workstation
cs_dv_status | `falcon_device.status` | normal
cs_sys_mf | `falcon_device.system_manufacturer` | hp
cs_sys_name | `falcon_device.system_product_name` | hp_elitebook_850_g7_notebook_pc
cs_external_ip | `falcon_device.external_ip` | 0.0.0.0
cs_tags | `falcon_device.tags{}` | n/a

Full example of category value

```text
cs_agent_version:6.40.15406.0
cs_bios_mf:hp
cs_bios_version:s73_ver_01.08.00
cs_dv_control_applied:true
cs_dv_firewall_applied:true
cs_dv_globalconfig_applied:true
cs_dv_sensorupdate_applied:true
cs_dv_status:normal
cs_dv_type:workstation
cs_external_ip:0.0.0.0
cs_os_major_version:10
cs_os_name:windows_10
cs_os_platform:windows
cs_sys_mf:hp
cs_sys_name:hp_elitebook_850_g7_notebook_pc
cs_uninstallprotection:enabled
```
