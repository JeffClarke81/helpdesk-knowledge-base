# Map a Network Drive on Windows

## Problem
User needs access to a shared network folder but cannot see it in File Explorer.

----------
## Possible Causes
- Network path not mapped
- Incorrect permissions
- Not connected to company network/VPN
- Network discovery disabled
- Incorrect credentials

----------
## Step-by-Step Resolution

### 1. Verify Network Connectivity
- Ensure the computer is connected to the network
- If remote, confirm VPN is connected
- Try pinging the file server (if known)

** Expected Results:** System is connected to the network.
----------

### 2. Obtain the Network Path
Confirm the correct shared folder path from the network.
 ** Example format:** \servername\sharedfolder

 **Expected Results:** Valid UNC path is available.
 ----------

 ### 3. Open Map Network Drive
 1. Open **File Explorer**
 2. Click **This PC**
 3. Select **Map network drive** from the top menu

** Expected Results:** Map Network Drive window opens.

----------

### 4. Choose Drive Letter and Folder
1. Select an available **Drive letter**
2. In the **Folder** field, enter the network path: \serverpath\sharedfolder
3. Check **Reconnect at sign-in** (recommended)
4. Click **Finish**

**Expected Results:** System attempts to connect to the shared drive.

----------

### 5. Enter Credentials (If Prompted)
- Enter domain or server credentials if required
- Optionally check **Remember my credentials**

**Expected Results:**  Authentication succeeds and drive connects.

----------

## Verification
- Open **File Explorer**
- Confirm the new network drive appears under **This PC**
- Open the drive and verify files are accessible

-----------

## Common Issues & Fixes

**Access Denied**
- Verify user permission on the shared folder
- Confirm correct username format (Domain\Username)

**Network Path Not Found**
- Verify server name spelling
- Confirm VPN connection if remote
- Test connectivity with ping

**Drive Disconnects After Reboot**
- Ensure **Reconnect at sign-in** is checked
- Verify network is available at login

----------

## Escalation Path
If the issue continues:

- Verify share permission on the server
- Confirm DNS resolution for the server
- Check firewall settings
- Escalate to system/network administrator

----------

## Notes
- Steps apply to Windows 10 and Windows 11
- Administrator rights may be required in some environments
