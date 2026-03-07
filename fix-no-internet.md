# Fix No Internet Connection on Windows

## Problem
User cannot access the internet. web browser shows "No internet" or pages fail to load.

----------
## Possible Causes
- Network adapter disabled
- Incorrect IP configuration
- DNS resolution failure
- Router or modem issues
- Outdated network drivers

----------
## Step-by-Step Resolution
### 1. Check Physical Connection
- Ensure the Ethernet cable is firmly connected (if using wired)
- Verify Wi-Fi is turned on
- Confirm Airplane mode is OFF

----------
### 2. Run Windows Network Troubleshooter
1. Open **Settings**
2. Go to **Network & Internet**
3. Click **Status**
4. Select **Network Troubleshooter**
6. Follow the prompts

**Expected Result:** Windows detects and fixes common issues.
----------
### 3. Restart Network Adapter
1. Press **Windows + R**
2. Type: ncpa.cpl
3. Right-click your active network adapter
4. Click **Disable**
5. Wait 10 seconds
6. Right-click again -> **Enable**

**Expected Result:** Network reconnects.
----------
### 4. Renew IP Address
1. Open **Command Prompts** as Administrator
2. Run the following command: ipconfig /release, ipconfig/renew

 **Expected results:** New IP address assigned.
----------
### 5. Flush DNS Cache
In Command Prompt, run: ipconfig /flushdns

** Expected Results:** DNS resolver cache cleared successfully.
----------
### 6. Restart the Computer
Reboot the system to ensure all network services reset.

**Expected results:** Internet connectivity restored.
----------
## Verification
- Open a web browser
- Navigate to a known website (example: google.com)
- Confirm pages load normally

----------
## Escalation Path
If the issue continues:

- Test another device on the same network
- Power cycle the modem/router
- Update network drivers
- Contact ISP if outage suspected

----------

## Notes
- Steps apply to Windows 10 and Windows 11
- Administrator access may be required for some commands
