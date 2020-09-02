# Zabbix Monitoring - vCenter 6.7 Appliance 

Copy the vcsa_discovery to "/usr/lib/zabbix/externalscripts" and update "vCenter IP" with the IP address of your vcenter Appliance.

Run the following command to set the permissions on the vcsa_discovery file

`sudo chmod a+x /usr/lib/zabbix/externalscripts/vcsa_discovery`

Import the Zabbix_4.0_vCenter_SNMP-VMWARE_VCSA_6.7.xml template in to your Zabbix Server.

Assign to you vCenter host and allow the discovery to complete.

Macro's Required:

`{$SNMP_COMMUNITY} = Public`

`{$SNMP_PORT} = 161`

SNMP needs to be enabled on your vcenter applience See [here](https://docs.vmware.com/en/VMware-vSphere/6.5/com.vmware.vsphere.vcsa.doc/GUID-AC191A28-2739-4250-A8CA-DCD7F4053ECE.html) for more info!

GLHF!
