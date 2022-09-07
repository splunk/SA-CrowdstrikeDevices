# Business Unit Field (bunit)

!!! info "To update the `bunit` field modify the `Crowdstrike Devices Lookup - Gen` saved search. It is recommended to clone the default search before making changes (see [Clone Saved Search](../best-practice/clone-search))."

The bunit field will most likely need to be updated. Every organization will have different values for this field. The current configuration is described in the following table.

Mapped Field | Crowdstrike fields
------------ | -----------------
bunit | `falcon_device.ou{}`, `falcon_device.site_name`
