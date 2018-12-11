# Overview
Real-time performance monitoring of multiple shared VMware VMFS datastores using PowerShell. The script uses VMware PowerCLI  to get read/ write IOPS and latency details of these shared datastores across all nodes in the cluster. Output format is given in the sample screenshot below and gets refreshed automatically every few seconds.

# How to use?
PS> .\Datastore_Stats.ps1 -vcenter [vcenter IP]

# Sample screenshot of output
![image](https://user-images.githubusercontent.com/30316226/49784524-37dff500-fce3-11e8-970f-373ded62dc35.png)

# Notes
"datastore_list.txt" should contain the list of datastore names and "esxi_list.txt" should contain the list of ESXi server names that needs to be monitored. And "datastore_list.txt" and "esxi_list.txt" files should be present in the same directory where this PS script is saved. In this case vol01, vol02 and vol03 are the 3 VMFS datastores shared across 3 ESXi nodes 192.168.105.10/11/12.
