# 06 - Shared Folder Configuration

## Objective
To establish file sharing between the Windows host machine and Kali Linux virtual machine.

## Configuration Requirements

- Host Operating System: Windows 11
- Guest Operating System: Kali Linux
- Shared Host Folder: Downloads
- Shared Folder Path in Kali Linux: /media/sf_Downloads

## Configuration Procedure

### Step 1: Open VirtualBox Settings
1. Shut down Kali Linux if required.
2. Open the Kali Linux VM settings.
3. Navigate to Shared Folders.

### Step 2: Add Shared Folder
1. Select Add Shared Folder.
2. Browse and select the host Downloads folder.
3. Set the folder name to Downloads.
4. Enable Auto-mount.
5. Enable Make Permanent.
6. Save the configuration.

### Step 3: Configure Clipboard
1. Open VM settings.
2. Navigate to General → Advanced.
3. Enable Shared Clipboard.
4. Select Bidirectional.

### Step 4: Configure Drag and Drop
1. Open General → Advanced.
2. Enable Drag and Drop.
3. Select Bidirectional.

### Step 5: Verify Shared Folder
Open Kali Linux terminal:

```bash
ls /media/sf_Downloads
```

Check whether the shared folder contents are accessible.

## Verification
The shared Downloads folder should be accessible from Kali Linux.

## Screenshots
Save screenshots in:

`screenshots/verification/`

## Result
Host-to-guest shared folder configuration documentation.