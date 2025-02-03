# Startup disabled by group policy

Your PC’s administrator or certain applications may disable startup for all apps in Windows. By modifying the Windows Registry, you can enable Full Trust and UWP Startup Tasks. This will allow you to choose MagicPods and other apps to start automatically after Windows loads.

1. Open the Registry Editor  
    1. Press `Win + R` on your keyboard.  
    2. In the `Run` dialog box, type `regedit` and press `Enter`.  
    3. If a `User Account Control (UAC)` prompt appears, click `Yes` to allow changes.  
2. Navigate to the Following Path  
    Copy and paste this path into the Registry Editor's address bar, then press Enter:   
    
    `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System`

3. Create or Modify the Required Values  
    You need to ensure the following `DWORD (32-bit) values` exist and have the correct settings:

    | Name                         | Type           | Value |
    | ---------------------------- | -------------- | ----- |
    | EnableFullTrustStartupTasks  | DWORD (32-bit) | 2     |
    | EnableUwpStartupTasks        | DWORD (32-bit) | 2     |
    | SupportFullTrustStartupTasks | DWORD (32-bit) | 1     |
    | SupportUwpStartupTasks       | DWORD (32-bit) | 1     |

    How to Modify an Existing Value

    1. In the `right pane`, look for the value you want to change.  
    2. `Double-click` on it.  
    3. In the `Value data` field, enter the correct number from the table above.  
    4. Click `OK`.  

    How to Create a New Value (If It’s Missing)

    1. Right-click in the `right pane` (empty space).  
    2. Select `New → DWORD (32-bit) Value`.  
    3. Type the name exactly as shown in the table (e.g., `EnableFullTrustStartupTasks`).  
    4. Press `Enter` to save the name.  
    5. `Double-click` the new entry.  
    6. In the `Value data` field, enter the correct number from the table.  
    7. Click `OK`.  

4. Save and Restart Your Computer