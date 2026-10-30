# 05 - Kali Linux IP Configuration

## Objective
To configure the network interface of Kali Linux according to the lab requirements.

## Required Network Configuration

| Parameter | Value |
|---|---|
| Network Type | NAT Network |
| Subnet | 10.0.0.0/24 |
| Kali Linux IP Address | 10.0.0.2/24 |

## Configuration Procedure

### Step 1: Configure VirtualBox Network
1. Open Kali Linux VM settings.
2. Navigate to Network.
3. Enable the network adapter.
4. Select NAT Network.
5. Choose the custom NAT Network created for the lab.
6. Save the settings.

### Step 2: Configure Kali Linux IP
Configure the Kali Linux network interface according to the required lab IP address:

10.0.0.2/24

### Step 3: Verify IP Configuration

Open the Kali Linux terminal and run:

```bash
ip addr
```

Check the active network interface and confirm the assigned IP address.

You can also run:

```bash
ip route
```

to inspect the routing configuration.

## Verification
- Kali Linux is connected to the custom NAT Network.
- The configured IP address matches the lab requirement.
- Network interface and routing information are checked.

## Screenshots
Save screenshots in:

`screenshots/kali-linux/`

## Result
Kali Linux IP configuration documentation.