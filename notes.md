#### Userful commands:
<details>

<summary>show system info</summary>

```
admin@Netlab-PA> show system info

hostname: Netlab-PA
ip-address: 10.255.255.128
public-ip-address: unknown
netmask: 255.255.255.0
default-gateway: 10.255.255.1
ip-assignment: dhcp
ipv6-address: unknown
ipv6-link-local-address: fe80::20c:29ff:fec9:b5b7/64
ipv6-default-gateway:
mac-address: 00:0c:29:c9:b5:b7
time: Sun Jun 29 04:46:46 2025
uptime: 0 days, 0:23:47
family: vm
model: PA-VM
serial: unknown
vm-mac-base: BA:DB:EE:FB:AD:00
vm-mac-count: 255
vm-uuid: 564D903C-CB33-D89C-877A-76476CC9B5B7
vm-cpuid: ESX:A3060B00FFFB8B1F
vm-license: none
vm-cap-tier: unknown
vm-cpu-count: 2
vm-memory: 8158328
vm-mode: VMware ESXi
cloud-mode: non-cloud
sw-version: 11.0.0
global-protect-client-package-version: 0.0.0
device-dictionary-version: 1-211
device-dictionary-release-date:
app-version: 8635-7675
app-release-date:
av-version: 0
av-release-date:
threat-version: 0
threat-release-date:
wf-private-version: 0
wf-private-release-date: unknown
url-db: paloaltonetworks
wildfire-version: 0
wildfire-release-date:
wildfire-rt: Disabled
url-filtering-version: 0000.00.00.000
global-protect-datafile-version: unknown
global-protect-datafile-release-date: unknown
global-protect-clientless-vpn-version: 0
global-protect-clientless-vpn-release-date:
logdb-version: 11.0.0
dlp: dlp-4.0.0
vm_series: vm_series-4.0.0
platform-family: vm
vpn-disable-mode: off
multi-vsys: off
operational-mode: normal
advanced-routing: off
device-certificate-status: None

admin@Netlab-PA>
```
</details>

<details>

<summary>show dhcp client mgmt-interface-state</summary>

```
admin@Netlab-PA> show dhcp client mgmt-interface-state

hostname: Netlab-PA
ip: 10.255.255.128
netmask: 255.255.255.0
default-gateway: 10.255.255.1
expiry-time: 2025/06/29 05:48:28 PDT
lease-time: 0 days, 00:30:00
dhcp-server: 10.255.255.254
domain: unknown
dns-server: unknown

admin@Netlab-PA>
```

</details>

<details>
  
<summary>request dhcp client management-interface renew</summary>

```
admin@Netlab-PA> request dhcp client management-interface renew
Warning: Performing DHCP Renew can cause firewall's management IP to change and access to firewall can be lost.  A console connection can be used to recover access if available. Do you wish to continue? (y or n)
DHCP: new ip 10.255.255.128 : mask 255.255.255.0
DHCP: new ip 10.255.255.128 : mask 255.255.255.0

Renew succeeded
admin@Netlab-PA>
```
</details>

<details>
  
<summary>show interface all</summary>

```
admin@Netlab-PA> show interface all

total configured hardware interfaces: 4

name                    id    speed/duplex/state            mac address
--------------------------------------------------------------------------------
ethernet1/1             16    1000/full/up                  00:0c:29:c9:b5:c1
ethernet1/2             17    1000/full/up                  00:0c:29:c9:b5:d5
ethernet1/3             18    1000/full/up                  00:0c:29:c9:b5:df
ethernet1/4             19    1000/full/up                  00:0c:29:c9:b5:cb

aggregation groups: 0


total configured logical interfaces: 4

name                id    vsys zone             forwarding               tag    address                                
------------------- ----- ---- ---------------- ------------------------ ------ ------------------
ethernet1/1         16    1    Untrusted-Outsid vr:default               0      13.1.87.6/29
ethernet1/2         17    1    Untrused-DMZ     vr:default               0      192.168.255.5/24
ethernet1/3         18    1    Trusted-LAN      vr:default               0      10.0.1.5/24
ethernet1/4         19    1    Trusted-LAN      vr:default               0      10.0.2.5/24

admin@Netlab-PA>
```

</details>

<details>
  
<summary>set cli config-output-format set</summary>

</details>

<details>
  
<summary>set cli config-output-format json</summary>

</details>
