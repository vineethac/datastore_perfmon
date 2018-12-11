# Overview
Real-time performance monitoring of multiple shared VMware datastores using PowerShell. The script which uses VMware PowerCLI  to get read/ write IOPS and latency details of these shared datastores across all nodes in the cluster. Output format is given in the sample screenshot below and gets refreshed automatically every few seconds.

# How to use?
PS> .\Datastore_Stats.ps1 -vcenter [vcenter IP]

# Sample screenshot of output
