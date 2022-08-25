# Business Unit Field (bunit)

!!! info "To update the `bunit` field modify the `Crowdstrike Devices Lookup - Gen` saved search."

The bunit field will most likely need to be updated. Every organization will have different values for this field. The current configuration is described in the following table.

Mapped Field | Crowdstrike field
------------ | -----------------
bunit | `falcon_device.ou{}`
