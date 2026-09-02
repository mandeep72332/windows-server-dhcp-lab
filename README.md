# windows-server-dhcp-lab
Windows Server DHCP configuration and high availability lab
# Windows Server DHCP Lab

## Project Overview

This project demonstrates the configuration and management of Dynamic Host Configuration Protocol (DHCP) in a Windows Server environment.

The lab covers DHCP Server installation, DHCP scope configuration, DHCP reservations, packet capture using Wireshark, DHCP policies, scope options, MAC address filtering, backup and restore, and DHCP high availability using failover.

## Technologies Used

* Windows Server
* Active Directory
* DHCP Server
* DNS
* Wireshark
* Windows Command Prompt

## Lab Components

### 1. DHCP Server Installation

The DHCP Server role was installed and configured on the Windows Server Domain Controller.

After installation, DHCP configuration was completed and DHCP Administrator and DHCP Users groups were available in Active Directory.

### 2. DHCP Scope Configuration

A new DHCP scope was created to dynamically assign IP addresses to devices on the network.

The DHCP scope was activated after configuration.

### 3. DHCP Lease Assignment

A Windows Server client was configured to obtain an IP address automatically.

The DHCP Server successfully assigned an IP address to the client.

### 4. DHCP Reservations

A DHCP reservation was configured to ensure that a specific device receives the same IP address whenever it requests an address dynamically.

### 5. Wireshark DHCP Packet Capture

Wireshark was used to capture DHCP traffic.

The following commands were used on the client:

```text
ipconfig /release
ipconfig /renew
```

The packet capture demonstrated the DHCP communication process between the client and DHCP Server.

### 6. DHCP Policies

A DHCP policy was configured to control network access based on defined conditions.

### 7. Scope Options

DHCP scope options were configured at the scope and server levels.

### 8. DHCP Filters

MAC address filtering was configured to allow or restrict network devices.

### 9. DHCP Backup

DHCP backup functionality was reviewed to support recovery if DHCP configuration or scopes are accidentally deleted.

### 10. DHCP High Availability

A second Windows Server was configured with the DHCP Server role.

DHCP failover was configured between the Domain Controller and the second Windows Server to provide DHCP availability.

The DHCP scope was replicated to the secondary DHCP Server.

## Skills Demonstrated

* Windows Server administration
* DHCP installation and configuration
* IP address management
* DHCP scopes and leases
* DHCP reservations
* DNS integration
* Network packet analysis with Wireshark
* DHCP policies and filtering
* Backup and recovery
* DHCP failover and high availability
* Network troubleshooting

## Documentation

Detailed lab documentation and screenshots are available in:

`documentation/DHCP-Mod1Sec4.docx`

## Project Structure

windows-server-dhcp-lab/
│
├── README.md
│
├── documentation/
│   └── DHCP-Mod1Sec4.docx
│
└── screenshots/

