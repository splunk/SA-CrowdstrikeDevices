# Quick Start

This add-on has a saved search and Asset configuration input enabled by default.

## Overview

1. [Updated default macro](#update-default-macro)
1. [Enable asset correlation](#enable-asset-correlation).
1. <small>(optional)</small> [Update default saved search schedule](#update-default-saved-search-schedule).
1. <small>(optional)</small> [Disable existing asset sources](#disable-existing-asset-sources).

## Update default macro

!!! danger "[Danger, Will Robinson](https://cultural-phenomenons.fandom.com/wiki/Danger,_Will_Robinson)"
    Failure to update the macro to the correct setting will cause the no devices to be available in Splunk Enterprise Security.

Macro | Default | Description
----- | ------- | -----------
`sa_crowdstrike_index` | index=crowdstrike | Index definition for Crowdstrike devices index.

> \*update the index definition to the correct index that contains the `crowdstrike:device:json` sourcetype.

### Update Macro Procedure

1. Navigate to Settings > Advanced Search > Search Macros.
1. From the "App" dropdown choose `SA-CrowdstrikeDevices`.
1. Set the "Owner" dropdown to `any`.
1. Click the macro named `sa_crowdstrike_index` to update the index definition.

## Enable asset correlation

Confirm asset correlation has been setup in Enterprise Security.

1. Navigate to Enterprise Security > Configure > Data Enrichment > Asset and Identity Management.
1. Switch to the "Correlation Setup" tab.
1. Either enable for all sourcetypes <small>(Recommended)</small> or selectively by sourcetype.
    - If you choose to enable select sourcetypes, ensure the `stash` sourcetype is also selected so Notable events will be enriched with asset information.
1. Save.

## Disable existing asset sources

!!! info "optional"

It may be possible that you have existing Asset Lookups defined. If Crowdstrike is widely deployed in your environment the other existing lookups may no longer be needed.

## Update default saved search schedule

!!! info "optional"

The default saved search runs on the 19th minute of every hour to update and continually build the Crowdstrike assets. To update the default schedule perform the following steps:

1. Navigate to Settings > Searches, reports, and alerts.
1. Set the "App" dropdown to `SA-CrowdstrikeDevices`.
1. Set the "Owner" dropdown to `All`.
1. Click "Edit" under actions for the search `Crowdstrike Devices Lookup - Gen`.
1. Click "Edit Schedule" and update the schedule and necessary.
