# Install

!!! important
    This supporting add-on must be installed alongside Splunk Enterprise Security. Ensure the [prequisites](../prerequisites) have been completed before proceeding.

For detailed information on where to install Splunk Apps/add-ons, including best practices, can be found at [Splunk Docs: About Installing Splunk add-ons](https://docs.splunk.com/Documentation/AddOns/released/Overview/Wheretoinstall)

## Standalone Deployments (with Splunk ES)

Install this add-on to the single instance. For more information see [Splunk Docs: Install add-on in a single-instance Splunk deployment](https://docs.splunk.com/Documentation/AddOns/released/Overview/Singleserverinstall)

## Distributed Deployments

Splunk Instance type | Supported | Required | Comments
-------------------- | --------- | -------- | --------
Enterprise Security Search Head | Yes | Yes | Install this add-on to the Enterprise Security Search Head.
Splunk Core Search Head (without ES) | No | No | Do not install on regular search heads.
Indexers | No | No | Do not install on Indexers.
Heavy Forwarders | No | No | Do not install on Heavy Forwarders.
Universal Forwarders | No | No | Do not install on Universal Forwarders.

The installation steps for deploying Apps/add-ons in a distributed environment can be found at [Splunk Docs: Install an add-on in a distributed Splunk deployment](https://docs.splunk.com/Documentation/AddOns/released/Overview/Distributedinstall)

## Distributed Deployment Compatibility

Distributed deployment feature | Supported | Comments
------------------------------ | --------- | --------
Search Head Clusters | Yes | You can install this add-on to an Enterprise Security search head cluster.
Indexer Clusters | No | Do not deploy this add-on to an Indexer cluster.
Deployment Server | No | There is no need to use a deployment server to deploy this add-on.

\* For more information, see Splunk's [documentation](https://docs.splunk.com/Documentation/AddOns/released/Overview/Installingadd-ons) on installing Add-ons.
