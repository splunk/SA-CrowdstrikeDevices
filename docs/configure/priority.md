# Priority Field

!!!primary To update the `priority` field modify the `Crowdstrike Devices Lookup - Gen` saved search. It is recommended to clone the default search before making changes (see [Clone Saved Search](clone-search.md)).
!!!

The priority field is very generic by default and should be updated to suite your environment. The following table describes how this field is set.

Type | Condition | Severity | Description
---- | --------- | -------- | -----------
RegEx\* | domain_controller | `critical` | All domain controllers
RegEx\* | server\|ubuntu\|rhel\|linux | `high` | Servers
boolean | true() | `medium` | catch-all. Remaining devices receive medium severity.


> \*Regex Match is performed on the category field.

Default priority field definition

```python
priority=case(
    match(category, "(?i)domain_controller"), "critical",
    match(category, "(?i)server|ubuntu|rhel|linux"), "high",
    true(), "medium"
    )
```
