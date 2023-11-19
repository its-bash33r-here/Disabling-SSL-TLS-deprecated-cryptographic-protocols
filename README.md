# Disabling SSL,TLS deprecated cryptographic protocols 
This is a step-by-step guide on how to disable SSL 2.0, SSL 3.0, TLS 1.0, and TLS 1.1 in Windows

## Step 1: Launch Registry Editor
1. Press Windows key + R
2. Type "regedit" and press Enter
3. Click "Yes" to confirm the UAC prompt

## Step 2: Navigate to the SChannel registry key
1. In the Registry Editor, expand the following keys:
    HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders

2. Select the "SCHANNEL" key

## Step 3: Disable SSL 2.0
1. Right-click the "SCHANNEL" key and select "New" > "DWORD (32-bit) Value"
2. Name the new value "SSL2.0" and press Enter
3. Double-click the "SSL2.0" value
4. In the Value data field, type "0" (zero) and click "OK"

## Step 4: Disable SSL 3.0
1. Right-click the "SCHANNEL" key and select "New" > "DWORD (32-bit) Value"
2. Name the new value "SSL3.0" and press Enter
3. Double-click the "SSL3.0" value
4. In the Value data field, type "0" (zero) and click "OK"

## Step 5: Disable TLS 1.0
1. Right-click the "SCHANNEL" key and select "New" > "DWORD (32-bit) Value"
2. Name the new value "TLS1.0" and press Enter
3. Double-click the "TLS1.0" value
4. In the Value data field, type "0" (zero) and click "OK"

## Step 6: Disable TLS 1.1
1. Right-click the "SCHANNEL" key and select "New" > "DWORD (32-bit) Value"
2. Name the new value "TLS1.1" and press Enter
3. Double-click the "TLS1.1" value
4. In the Value data field, type "0" (zero) and click "OK"

## Step 7: Restart your computer
Restart your computer for the changes to take effect.

This repository contains a detailed guide on how to disable SSL 2.0, SSL 3.0, TLS 1.0, and TLS 1.1 in Windows 10 using the registry editor and Group Policy.
