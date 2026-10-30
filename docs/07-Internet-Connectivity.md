# 07 - Internet Connectivity Verification

## Objective
To verify internet connectivity from the Kali Linux virtual machine.

## Network Requirements

- NAT Network configuration
- Kali Linux IP: 10.0.0.2/24
- Working internet connection

## Verification Procedure

### Step 1: Check Network Interface

```bash
ip addr
```

### Step 2: Check Network Routing

```bash
ip route
```

### Step 3: Test Internet Connectivity

```bash
ping -c 4 google.com
```

### Step 4: Check DNS Resolution

```bash
nslookup google.com
```

## Expected Results

- Kali Linux should have a working network interface.
- Network routing should be configured.
- DNS resolution should work.
- Internet connectivity should be verified.

## Screenshots
Save verification screenshots in:

`screenshots/verification/`

## Result
Internet connectivity verification documentation for Kali Linux.