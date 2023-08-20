---
order: -3
icon: workflow
label: Force build
---

# Force initial build

!!!info Optional
!!!

The initial build of the Crowdstrike assets will not occur until the first scheduled runtime (see [Update default saved search schedule](#update-default-saved-search-schedule)). To force the initial build perform the following:

1. Navigate to Settings > Searches, reports, and alerts.
2. Set the "App" dropdown to `SA-CrowdstrikeDevices`.
3. Set the "Owner" dropdown to `All`.
4. Click "Run" under actions for the search `Crowdstrike Devices Lookup - Gen`.

!!!info Note
The search will run in a new tab over the default time period of 60 minutes. Expand the timeframe to a larger window if the number of hosts in the last 60 minutes does not seem accurate. The default search is configured to run hourly to continually append new devices reported from Crowdstrike.
!!!