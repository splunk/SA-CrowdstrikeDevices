---
order: -6
label: Update schedule
icon: clock
---

# Update default saved search schedule

!!!info Optional
!!!

The default saved search runs on the 19th minute of every hour to update and continually build the CrowdStrike assets. To update the default schedule perform the following steps:

==- :icon-star-fill: Use Enterprise Security's Settings <small>(Recommended)</small>
1. <small>(In Enterprise Security)</small> Navigate to Configure > Content > Content Management.
2. Type "SA-CrowdStrikeDevices" in the filter text box.
3. Click "SA-CrowdstrikeDevices"
4. Update the "Schedule" section as necessary
5. If necessary, the retention settings can be modified by changing the "Retention" at the bottom.
==- Update the Schedule Manually (For retention settings follow previous steps)
1. Navigate to Settings > Searches, reports, and alerts.
2. Set the "App" dropdown to `SA-CrowdstrikeDevices`.
3. Set the "Owner" dropdown to `All`.
4. Click "Edit" under actions for the search `CrowdStrike Devices Lookup - Gen`.
5.  Click "Edit Schedule" and update the schedule and necessary.
===