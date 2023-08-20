---
order: -4
icon: play
---

# Enable asset correlation

Confirm asset correlation has been setup in Enterprise Security.

1. Navigate to Enterprise Security > Configure > Data Enrichment > Asset and Identity Management.
1. Switch to the "Correlation Setup" tab.
1. Either enable for all sourcetypes <small>(Recommended)</small> or selectively by sourcetype.
    - If you choose to enable select sourcetypes, ensure the `stash` sourcetype is also selected so Notable events will be enriched with asset information.
1. Save.

---

## Disable existing asset sources

!!! info Optional
!!!

It may be possible that you have existing Asset Lookups defined. If Crowdstrike is widely deployed in your environment the existing lookups may no longer be needed.