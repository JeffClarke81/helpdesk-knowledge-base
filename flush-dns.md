# Flush DNS Cache on Windows

## Problem
User can access the internet, but specific websites fail to load, load the wrong site, or show DNS-related errors.

----------

## Possible Causes
- Corrupted DNS cache
- Recent DNS changes not updated locally
- Website IP address changed
- Browser showing outdated records

----------

## Step-by-Step Resolution

### 1. Open Command Prompt as Administrator
1. Click **Start**
2. Type **cmd**
3. Right-click **Command Prompt**
4. Select **Run as administrator**

**Expected Result:** Elevated Command Prompt window opens.

----------

### 2. Flush the DNS Cache
In Command Prompt, run: ipconfig /flushdns
press **Enter**.

**Expected Result:** Message displays:
> Successfully flushed the DNS Resolver Cache.

----------

### 3. Test Website Access
- Open a web browser
- Navigate to the affected website
- Refresh the page (CTRL + F5 recommended)

**Expected Result:** Website loads correctly.

----------

## Verification
- No DNS errors appear
- Website resolves to the correct page
- User confirms normal browsing

----------

## Common Issues & Fixes

**Access Denied**
- Ensure Command Prompt is run as Administrator

**Flush Appears Successful, but Issue Persists**
- Clear browser cache
- Try a different browser
- Restart the computer
- Verify DNS server settings

**Still Cannot Reach Site**
- Test with: nslookup example.com
- Check network connectivity
- Verify the site is not down

----------

## Escalation Path
If the issue continues:

- Change DNS server (e.g., to public DNS)
- Check firewall or security software
- Verify no network-wide DNS issues
- Escalate to the network administrator

----------

## Notes
- Applies to Windows 10 and Windows 11
- Requires administrator privileges
- Common first step for name resolution issues
