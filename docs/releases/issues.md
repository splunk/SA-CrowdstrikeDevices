---
icon: bug
order: -100
---

# Known issues

Issue | Description | Solution 
----- | ----------- | --------
Lookup file error | You may see the error `status="Lookup file error, unknown path or update time" name=crowdstrike_devices` | This error exists since the KVstore is being used opposed to a csv file and does not interfere with the functionality of lookup creation. <br><br>You can tune out name field (crowdstrike_devices) from saved search: Identity - Identity Manager Error to stop the error messages from this source.
