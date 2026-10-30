# 03 - NAT Network Configuration

## Objective
To create a custom NAT Network in Oracle VirtualBox for the cybersecurity testing lab.

## Network Configuration

| Parameter | Value |
|---|---|
| Network Type | NAT Network |
| Network Name | Custom NAT Network1 |
| Network Subnet | 10.0.0.0/24 |
| Network Range | 10.0.0.2 - 10.0.0.99 |

## Configuration Procedure

1. Open Oracle VirtualBox.
2. Navigate to the Network settings.
3. Open the NAT Networks section.
4. Create a new NAT Network.
5. Configure the network subnet as 10.0.0.0/24.
6. Configure the address range as specified in the lab instructions.
7. Save the network configuration.
8. Attach the Kali Linux VM to this NAT Network.

## Verification

Verify that:
- The NAT Network is created.
- The subnet is configured correctly.
- The Kali Linux VM is connected to the NAT Network.

## Screenshots

Save relevant screenshots in:

`screenshots/network/`

## Result

NAT Network configuration documentation for the cybersecurity lab.