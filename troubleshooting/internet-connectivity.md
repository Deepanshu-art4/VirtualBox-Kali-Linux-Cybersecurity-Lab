# Internet Connectivity Troubleshooting

## Problem
Kali Linux VM may experience internet connectivity issues while using VirtualBox NAT Network.

## Checks Performed

1. Verify that the Kali VM is connected to the correct NAT Network.
2. Check the IP address and network interface.
3. Verify that no other VM is using the same static IP address.
4. Check the network configuration in VirtualBox.

## Network Configuration

- NAT Network: NatNetwork1
- IPv4 Subnet: 10.0.0.0/24
- Kali Linux IP: 10.0.0.2/24

## Network Commands

Run these commands in the Kali terminal:

```bash
ip addr
ip route
ping -c 4 8.8.8.8
ping -c 4 google.com
```

## Network Connection Reset

If the network connection requires troubleshooting, run:

```bash
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
sudo nmcli connection down "Wired connection 1"
sudo nmcli connection up "Wired connection 1"
```

## Verification

- Check whether the network interface is active.
- Check whether the expected IP address is assigned.
- Test connectivity using an IP address.
- Test DNS resolution using a domain name.

## Result

The Kali Linux VM successfully received the configured IP address and internet connectivity was verified using ping tests.

## Screenshots

See the `screenshots/kali-linux/` and `screenshots/verification/` folders for supporting evidence.