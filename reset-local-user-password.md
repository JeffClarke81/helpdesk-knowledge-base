# Reset a Local User Password on Windows

## Problem
A user cannot log in to their Windows account because they forgot their password or because their password is no longer accepted.

----------

## Possible Causes
- Forgotten password
- Password recently changed
- Account locked out
- Incorrect keyboard input (Caps Lock, Num Lock)

----------

## Step-by_Step Resolution

### 1. Log in with Administrator Account
To reset a local  password, you must be logged into a Windows account with **administrator privileges**.

**Expected Result:** Access to the Windows desktop with administrator rights.

----------

### 2. Open Computer Management
1. Press **Windows + X**
2. Click **Computer Management**

Alternative method:
1. Press **Windows + R**
2. Type: compmgmt.msc
3. Press Enter

**Expected Result:** Computer Management console opens.

----------

### 3. Navigate to Local Users
In the left panel:

1. Expand **Local Users and groups**
2. Click **Users**

You will see a list of local accounts.

**Expected Result:** All local user accounts appear.

----------

### 4. Reset the Password
1. Right-click the user account that needs the password reset
2. Select **Set Password**
3. Click **Proceed** when the warning appears
4. Enter the new password
5. Confirm the password
6. Click **OK**

**Expected Result:** Password successfully updated.

----------

### 5. Inform the User
Advise the user to log in using the new password.

**Expected Result:** User successfully logs into their account.

----------

## Verification
- The user can log into Windows with the new password
- No login errors appear
- User profile loads normally

----------

## Common Issues & Fixes

**Access Denied**
- Ensure the account performing the reset had administrator privileges

**Local Users and Groups Missing**
- This feature may not be available in Windows Home editions

**Account Locked**
- Wait for the lockout Timer to expire or unlock through account settings

----------

## Escalation Path
If the password cannot be reset:
- Verify administrator permissions
- Use an alternate account
- Escalate to the systems administrator if the domain account is involved

----------

## Notes
- Applies to Windows 10 and Windows 11
- Only works for **local accounts**, not domain accounts
