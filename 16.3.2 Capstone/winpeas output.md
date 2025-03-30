```
[33m [!] If you want to run the file analysis checks (search sensitive information in files), you need to specify the 'fileanalysis' or 'all' argument. Note that this search might take several minutes. For help, run winpeass.exe --help[0m
ANSI color bit for Windows is not set. If you are executing this from a Windows terminal inside the host you should run 'REG ADD HKCU\Console /v VirtualTerminalLevel /t REG_DWORD /d 1' and then start a new CMD
Long paths are disabled, so the maximum length of a path supported is 260 chars (this may cause false negatives when looking for files). If you are admin, you can enable it with 'REG ADD HKLM\SYSTEM\CurrentControlSet\Control\FileSystem /v VirtualTerminalLevel /t REG_DWORD /d 1' and then start a new CMD
[34m     
               [1;32m((((((((((((((((((((((((((((((((
        [1;32m(((((((((((((((((((((((((((((((((((((((((((
      [1;32m(((((((((((((([34m**********/[1;32m##########[1;32m(((((((((((((   
    [1;32m(((((((((((([34m********************/[1;32m#######[1;32m(((((((((((
    [1;32m(((((((([34m******************[0m/@@@@@/[1;32m[34m****[1;32m######[1;32m((((((((((
    [1;32m(((((([34m********************[0m@@@@@@@@@@/[1;32m[34m***,[1;32m####[1;32m((((((((((
    [1;32m((((([34m********************[0m/@@@@@%@@@@/[1;32m[34m********[1;32m##[1;32m(((((((((
    [1;32m((([1;32m############[34m*********[0m/%@@@@@@@@@/[1;32m[34m************[1;32m((((((((
    [1;32m(([1;32m##################(/[34m******[0m/@@@@@/[1;32m[34m***************[1;32m((((((
    [1;32m(([1;32m#########################(/[34m**********************[1;32m(((((
    [1;32m(([1;32m##############################(/[34m*****************[1;32m(((((
    [1;32m(([1;32m###################################(/[34m************[1;32m(((((
    [1;32m(([1;32m#######################################([34m*********[1;32m(((((
    [1;32m(([1;32m#######(,.***.,(###################(..***.[34m*******[1;32m(((((
    [1;32m(([1;32m#######*(#####((##################((######/([34m*****[1;32m(((((
    [1;32m(([1;32m###################(/***********(##############([1;32m)(((((
    [1;32m((([1;32m#####################/*******(################[1;32m)((((((
    [1;32m(((([1;32m############################################[1;32m)((((((
    [1;32m((((([1;32m##########################################[1;32m)(((((((
    [1;32m(((((([1;32m########################################[1;32m)(((((((
    [1;32m(((((((([1;32m####################################[1;32m)((((((((
    [1;32m((((((((([1;32m#################################[1;32m)(((((((((
        [1;32m(((((((((([1;32m##########################[1;32m)(((((((((
              [1;32m((((((((((((((((((((((((((((((((((((((
                 [1;32m(((((((((((((((((((((((((((((([0m

[1;33mADVISORY: [34mwinpeas should be used for authorized penetration testing and/or educational purposes only.Any misuse of this software will not be the responsibility of the author or of any other collaborator. Use it at your own devices and/or with the device owner's permission.

[33m  WinPEAS-ng[0m[33m by @hacktricks_live[0m
[1;32m
       /---------------------------------------------------------------------------------\
       |                             [34mDo you like PEASS?[1;32m                                  |
       |---------------------------------------------------------------------------------| 
       |         [33mLearn Cloud Hacking[1;32m       :     [1;31mtraining.hacktricks.xyz[1;32m                 |
       |         [33mFollow on Twitter[1;32m         :     [1;31m@hacktricks_live[1;32m                        |
       |         [33mRespect on HTB[1;32m            :     [1;31mSirBroccoli            [1;32m                 |
       |---------------------------------------------------------------------------------|
       |                                 [34mThank you![1;32m                                      |
       \---------------------------------------------------------------------------------/
[0m
[33m  [+] [1;32mLegend:[0m
[1;31m         Red[1;37m                Indicates a special privilege over an object or something is misconfigured[0m
[1;32m         Green[1;37m              Indicates that some protection is enabled or something is well configured[0m
[36m         Cyan[1;37m               Indicates active users[0m
[34m         Blue[1;37m               Indicates disabled users[0m
[1;33m         LightYellow[1;37m        Indicates links[0m

[34m You can find a Windows local PE Checklist here: [33mhttps://book.hacktricks.xyz/windows-hardening/checklist-windows-privilege-escalation
[1;90m   Creating Dynamic lists, this could take a while, please wait...[0m
[1;90m   - Loading sensitive_files yaml definitions file...[0m
[1;90m   - Loading regexes yaml definitions file...[0m
[1;90m   - Checking if domain...[0m
[1;90m   - Getting Win32_UserAccount info...[0m
[1;90m   - Creating current user groups list...[0m
[1;90m   - Creating active users list (local only)...[0m
[1;90m   - Creating disabled users list...[0m
[1;90m   - Admin users list...[0m
[1;90m   - Creating AppLocker bypass list...[0m
[1;90m   - Creating files/directories list for search...[0m


[1;36m════════════════════════════════════╣ [1;32mSystem Information[1;36m ╠════════════════════════════════════[0m

[1;36m╔══════════╣ [1;32mBasic System Information[0m
[1;36m╚ [1;34mCheck if the Windows versions is vulnerable to some known exploit [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#kernel-exploits[0m
[1;37m    OS Name: [0mMicrosoft Windows 11 Pro
[1;37m    OS Version: [0m10.0.22000 N/A Build 22000
[1;37m    System Type: [0mx64-based PC
[1;37m    Hostname: [0mclientwk222
[1;37m    ProductName: [0mWindows 10 Enterprise
[1;37m    EditionID: [0mEnterprise
[1;37m    ReleaseId: [0m2009
[1;37m    BuildBranch: [0mco_release
[1;37m    CurrentMajorVersionNumber: [0m10
[1;37m    CurrentVersion: [0m6.3
[1;37m    Architecture: [0mAMD64
[1;37m    ProcessorCount: [0m2
[1;37m    SystemLang: [0men-US
[1;37m    KeyboardLang: [0mEnglish (United States)
[1;37m    TimeZone: [0m(UTC-08:00) Pacific Time (US & Canada)
[1;37m    IsVirtualMachine: [0m[0m[1;31mTrue[0m
[1;37m    Current Time: [0m12/6/2024 8:15:55 AM
[1;37m    HighIntegrity: [0mFalse
[1;37m    PartOfDomain: [0mFalse
[1;37m    Hotfixes: [0m[1;32mKB5017024 (9/16/2022), KB5012170 (9/16/2022), KB5017328 (9/16/2022), KB5018291 (9/16/2022), [0m


[1;36m╔══════════╣ [1;32mShowing All Microsoft Updates[0m
   HotFix ID                :   KB2267602
   Installed At (UTC)       :   12/6/2024 11:07:52 PM
   Title                    :   Security Intelligence Update for Microsoft Defender Antivirus - KB2267602 (Version 1.421.654.0) - Current Channel (Broad)
   Client Application ID    :   Windows Defender
   Description              :   Install this update to revise the files that are used to detect viruses, spyware, and other potentially unwanted software. Once you have installed this item, it cannot be removed.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB2267602
   Installed At (UTC)       :   12/8/2022 7:30:24 AM
   Title                    :   Security Intelligence Update for Microsoft Defender Antivirus - KB2267602 (Version 1.381.75.0)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   Install this update to revise the files that are used to detect viruses, spyware, and other potentially unwanted software. Once you have installed this item, it cannot be removed.

[1;90m   =================================================================================================[0m

   HotFix ID                :   
   Installed At (UTC)       :   11/17/2022 3:20:10 AM
   Title                    :   9WZDNCRFJBBG-MICROSOFT.WINDOWSCAMERA
   Client Application ID    :   Update;ScanForUpdates
   Description              :   9WZDNCRFJBBG-1152921505695508168

[1;90m   =================================================================================================[0m

   HotFix ID                :   
   Installed At (UTC)       :   11/17/2022 3:19:55 AM
   Title                    :   9MSMLRH6LZF3-Microsoft.WindowsNotepad
   Client Application ID    :   Update;ScanForUpdates
   Description              :   9MSMLRH6LZF3-1152921505695502826

[1;90m   =================================================================================================[0m

   HotFix ID                :   
   Installed At (UTC)       :   11/17/2022 3:19:40 AM
   Title                    :   9WZDNCRFJ3P2-MICROSOFT.ZUNEVIDEO
   Client Application ID    :   Update;ScanForUpdates
   Description              :   9WZDNCRFJ3P2-1152921505695503140

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB2267602
   Installed At (UTC)       :   11/17/2022 3:00:51 AM
   Title                    :   Security Intelligence Update for Microsoft Defender Antivirus - KB2267602 (Version 1.379.444.0)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   Install this update to revise the files that are used to detect viruses, spyware, and other potentially unwanted software. Once you have installed this item, it cannot be removed.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB4052623
   Installed At (UTC)       :   11/17/2022 3:00:41 AM
   Title                    :   Update for Microsoft Defender Antivirus antimalware platform - KB4052623 (Version 4.18.2210.6)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   This package will update Microsoft Defender Antivirus antimalware platform's components on the user machine.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB2267602
   Installed At (UTC)       :   11/17/2022 3:00:02 AM
   Title                    :   Security Intelligence Update for Microsoft Defender Antivirus - KB2267602 (Version 1.379.379.0)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   Install this update to revise the files that are used to detect viruses, spyware, and other potentially unwanted software. Once you have installed this item, it cannot be removed.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB2267602
   Installed At (UTC)       :   11/16/2022 3:17:36 AM
   Title                    :   Security Intelligence Update for Microsoft Defender Antivirus - KB2267602 (Version 1.379.379.0)
   Client Application ID    :   Windows Defender
   Description              :   Install this update to revise the files that are used to detect viruses, spyware, and other potentially unwanted software. Once you have installed this item, it cannot be removed.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB2267602
   Installed At (UTC)       :   11/16/2022 3:13:22 AM
   Title                    :   Security Intelligence Update for Microsoft Defender Antivirus - KB2267602 (Version 1.379.379.0)
   Client Application ID    :   Windows Defender
   Description              :   Install this update to revise the files that are used to detect viruses, spyware, and other potentially unwanted software. Once you have installed this item, it cannot be removed.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB2267602
   Installed At (UTC)       :   9/22/2022 4:52:28 AM
   Title                    :   Security Intelligence Update for Microsoft Defender Antivirus - KB2267602 (Version 1.375.750.0)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   Install this update to revise the files that are used to detect viruses, spyware, and other potentially unwanted software. Once you have installed this item, it cannot be removed.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB5012170
   Installed At (UTC)       :   9/17/2022 12:58:00 AM
   Title                    :   2022-08 Security Update for Windows 11 for x64-based Systems (KB5012170)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   A security issue has been identified in a Microsoft software product that could affect your system. You can help protect your system by installing this update from Microsoft. For a complete listing of the issues that are included in this update, see the associated Microsoft Knowledge Base article. After you install this update, you may have to restart your system.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB5017328
   Installed At (UTC)       :   9/17/2022 12:29:48 AM
   Title                    :   2022-09 Cumulative Update for Windows 11 for x64-based Systems (KB5017328)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   Install this update to resolve issues in Windows. For a complete listing of the issues that are included in this update, see the associated Microsoft Knowledge Base article for more information. After you install this item, you may have to restart your computer.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB4052623
   Installed At (UTC)       :   9/16/2022 11:59:46 PM
   Title                    :   Update for Microsoft Defender Antivirus antimalware platform - KB4052623 (Version 4.18.2207.7)
   Client Application ID    :   Windows Defender
   Description              :   This package will update Microsoft Defender Antivirus antimalware platform's components on the user machine.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB2267602
   Installed At (UTC)       :   9/16/2022 11:52:59 PM
   Title                    :   Security Intelligence Update for Microsoft Defender Antivirus - KB2267602 (Version 1.375.449.0)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   Install this update to revise the files that are used to detect viruses, spyware, and other potentially unwanted software. Once you have installed this item, it cannot be removed.

[1;90m   =================================================================================================[0m

   HotFix ID                :   
   Installed At (UTC)       :   9/16/2022 11:45:49 PM
   Title                    :   VMware, Inc. - SCSIAdapter - 1.3.25.0
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   VMware, Inc. SCSIAdapter  driver update released in  March 2022

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB5017328
   Installed At (UTC)       :   9/16/2022 11:45:46 PM
   Title                    :   2022-09 Cumulative Update for Windows 11 for x64-based Systems (KB5017328)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   Install this update to resolve issues in Windows. For a complete listing of the issues that are included in this update, see the associated Microsoft Knowledge Base article for more information. After you install this item, you may have to restart your computer.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB5017328
   Installed At (UTC)       :   9/16/2022 11:45:39 PM
   Title                    :   2022-09 Cumulative Update for Windows 11 for x64-based Systems (KB5017328)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   Install this update to resolve issues in Windows. For a complete listing of the issues that are included in this update, see the associated Microsoft Knowledge Base article for more information. After you install this item, you may have to restart your computer.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB4023057
   Installed At (UTC)       :   9/16/2022 11:45:37 PM
   Title                    :   2022-04 Update for Windows 11 for x64-based Systems (KB4023057)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   A security issue has been identified in a Microsoft software product that could affect your system. You can help protect your system by installing this update from Microsoft. For a complete listing of the issues that are included in this update, see the associated Microsoft Knowledge Base article. After you install this update, you may have to restart your system.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB5017328
   Installed At (UTC)       :   9/16/2022 11:45:33 PM
   Title                    :   2022-09 Cumulative Update for Windows 11 for x64-based Systems (KB5017328)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   Install this update to resolve issues in Windows. For a complete listing of the issues that are included in this update, see the associated Microsoft Knowledge Base article for more information. After you install this item, you may have to restart your computer.

[1;90m   =================================================================================================[0m

   HotFix ID                :   
   Installed At (UTC)       :   9/16/2022 11:40:45 PM
   Title                    :   VMware, Inc. - Net - 1.9.9.0
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   VMware, Inc. Net  driver update released in  June 2022

[1;90m   =================================================================================================[0m

   HotFix ID                :   
   Installed At (UTC)       :   9/16/2022 11:40:41 PM
   Title                    :   VMware, Inc. - SCSIAdapter - 1.3.25.0
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   VMware, Inc. SCSIAdapter  driver update released in  March 2022

[1;90m   =================================================================================================[0m

   HotFix ID                :   
   Installed At (UTC)       :   9/16/2022 11:40:40 PM
   Title                    :   VMware, Inc. - System - 9.8.18.0
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   VMware, Inc. System  driver update released in  October 2021

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB890830
   Installed At (UTC)       :   9/16/2022 11:40:38 PM
   Title                    :   Windows Malicious Software Removal Tool x64 - v5.105 (KB890830)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   After the download, this tool runs one time to check your computer for infection by specific, prevalent malicious software (including Blaster, Sasser, and Mydoom) and helps remove any infection that is found. If an infection is found, the tool will display a status report the next time that you start your computer. A new version of the tool will be offered every month. If you want to manually run the tool on your computer, you can download a copy from the Microsoft Download Center, or you can run an online version from microsoft.com. This tool is not a replacement for an antivirus product. To help protect your computer, you should use an antivirus product.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB5017497
   Installed At (UTC)       :   9/16/2022 11:24:50 PM
   Title                    :   2022-09 Cumulative Update for .NET Framework 3.5, 4.8 and 4.8.1 for Windows 11 for x64 (KB5017497)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   A security issue has been identified in a Microsoft software product that could affect your system. You can help protect your system by installing this update from Microsoft. For a complete listing of the issues that are included in this update, see the associated Microsoft Knowledge Base article. After you install this update, you may have to restart your system.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB5017328
   Installed At (UTC)       :   9/16/2022 11:16:39 PM
   Title                    :   2022-09 Cumulative Update for Windows 11 for x64-based Systems (KB5017328)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   Install this update to resolve issues in Windows. For a complete listing of the issues that are included in this update, see the associated Microsoft Knowledge Base article for more information. After you install this item, you may have to restart your computer.

[1;90m   =================================================================================================[0m

   HotFix ID                :   KB5007651
   Installed At (UTC)       :   9/16/2022 11:13:48 PM
   Title                    :   Update for Windows Security platform - KB5007651 (Version 1.0.2207.20002)
   Client Application ID    :   MoUpdateOrchestrator
   Description              :   This package will update Windows Security platform components on the user machine.

[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mSystem Last Shutdown Date/time (from Registry)
[0m
    Last Shutdown Date/time        :    9/3/2024 5:53:13 AM

[1;36m╔══════════╣ [1;32mUser Environment Variables[0m
[1;36m╚ [1;34mCheck for some passwords or keys in the env variables [1;33m[0m
[1;37m    COMPUTER[0m[1;31mNAME[0m: [0mCLIENTWK222
[1;37m    USERPROFILE: [0mC:\Users\alex
[1;37m    HOMEPATH: [0m\Users\alex
[1;37m    LOCALAPPDATA: [0mC:\Users\alex\AppData\Local
[1;37m    PSModulePath: [0mC:\Users\alex\Documents\WindowsPowerShell\Modules;C:\Program Files\WindowsPowerShell\Modules;C:\Windows\system32\WindowsPowerShell\v1.0\Modules
[1;37m    PROCESSOR_ARCHITECTURE: [0mAMD64
[1;37m    Path: [0mC:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Windows\System32\OpenSSH\;C:\Users\alex\AppData\Local\Microsoft\WindowsApps;
[1;37m    CommonProgramFiles(x86): [0mC:\Program Files (x86)\Common Files
[1;37m    ProgramFiles(x86): [0mC:\Program Files (x86)
[1;37m    PROCESSOR_LEVEL: [0m23
[1;37m    LOGONSERVER: [0m\\CLIENTWK222
[1;37m    PATHEXT: [0m.COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC;.CPL
[1;37m    HOMEDRIVE: [0mC:
[1;37m    SystemRoot: [0mC:\Windows
[1;37m    [0m[1;31mSESSIONNAME[0m: [0mRDP-Tcp#0
[1;37m    ALLUSERSPROFILE: [0mC:\ProgramData
[1;37m    DriverData: [0mC:\Windows\System32\Drivers\DriverData
[1;37m    APPDATA: [0mC:\Users\alex\AppData\Roaming
[1;37m    PROCESSOR_REVISION: [0m0102
[1;37m    USER[0m[1;31mNAME[0m: [0malex
[1;37m    CommonProgramW6432: [0mC:\Program Files\Common Files
[1;37m    CommonProgramFiles: [0mC:\Program Files\Common Files
[1;37m    OneDrive: [0mC:\Users\alex\OneDrive
[1;37m    CLIENT[0m[1;31mNAME[0m: [0mkali
[1;37m    OS: [0mWindows_NT
[1;37m    USERDOMAIN_ROAMINGPROFILE: [0mCLIENTWK222
[1;37m    PROCESSOR_IDENTIFIER: [0mAMD64 Family 23 Model 1 Stepping 2, AuthenticAMD
[1;37m    ComSpec: [0mC:\Windows\system32\cmd.exe
[1;37m    SystemDrive: [0mC:
[1;37m    TEMP: [0mC:\Users\alex\AppData\Local\Temp
[1;37m    ProgramFiles: [0mC:\Program Files
[1;37m    NUMBER_OF_PROCESSORS: [0m2
[1;37m    TMP: [0mC:\Users\alex\AppData\Local\Temp
[1;37m    ProgramData: [0mC:\ProgramData
[1;37m    ProgramW6432: [0mC:\Program Files
[1;37m    windir: [0mC:\Windows
[1;37m    USERDOMAIN: [0mCLIENTWK222
[1;37m    PUBLIC: [0mC:\Users\Public

[1;36m╔══════════╣ [1;32mSystem Environment Variables[0m
[1;36m╚ [1;34mCheck for some passwords or keys in the env variables [1;33m[0m
[1;37m    ComSpec: [0mC:\Windows\system32\cmd.exe
[1;37m    DriverData: [0mC:\Windows\System32\Drivers\DriverData
[1;37m    OS: [0mWindows_NT
[1;37m    Path: [0mC:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Windows\System32\OpenSSH\
[1;37m    PATHEXT: [0m.COM;.EXE;.BAT;.CMD;.VBS;.VBE;.JS;.JSE;.WSF;.WSH;.MSC
[1;37m    PROCESSOR_ARCHITECTURE: [0mAMD64
[1;37m    PSModulePath: [0mC:\Program Files\WindowsPowerShell\Modules;C:\Windows\system32\WindowsPowerShell\v1.0\Modules
[1;37m    TEMP: [0mC:\Windows\TEMP
[1;37m    TMP: [0mC:\Windows\TEMP
[1;37m    USER[0m[1;31mNAME[0m: [0mSYSTEM
[1;37m    windir: [0mC:\Windows
[1;37m    NUMBER_OF_PROCESSORS: [0m2
[1;37m    PROCESSOR_LEVEL: [0m23
[1;37m    PROCESSOR_IDENTIFIER: [0mAMD64 Family 23 Model 1 Stepping 2, AuthenticAMD
[1;37m    PROCESSOR_REVISION: [0m0102

[1;36m╔══════════╣ [1;32mAudit Settings[0m
[1;36m╚ [1;34mCheck what is being logged [1;33m[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mAudit Policy Settings - Classic & Advanced[0m

[1;36m╔══════════╣ [1;32mWEF Settings[0m
[1;36m╚ [1;34mWindows Event Forwarding, is interesting to know were are sent the logs [1;33m[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mLAPS Settings[0m
[1;36m╚ [1;34mIf installed, local administrator password is changed frequently and is restricted by ACL [1;33m[0m
[1;37m    LAPS Enabled: [0m[0m[1;31mLAPS not installed[0m

[1;36m╔══════════╣ [1;32mWdigest[0m
[1;36m╚ [1;34mIf enabled, plain-text crds could be stored in LSASS [1;33mhttps://book.hacktricks.xyz/windows-hardening/stealing-credentials/credentials-protections#wdigest[0m
[1;32m    Wdigest is not enabled[0m

[1;36m╔══════════╣ [1;32mLSA Protection[0m
[1;36m╚ [1;34mIf enabled, a driver is needed to read LSASS memory (If Secure Boot or UEFI, RunAsPPL cannot be disabled by deleting the registry key) [1;33mhttps://book.hacktricks.xyz/windows-hardening/stealing-credentials/credentials-protections#lsa-protection[0m
[1;31m    LSA Protection is not enabled[0m

[1;36m╔══════════╣ [1;32mCredentials Guard[0m
[1;36m╚ [1;34mIf enabled, a driver is needed to read LSASS memory [1;33mhttps://book.hacktricks.xyz/windows-hardening/stealing-credentials/credentials-protections#credential-guard[0m
[1;31m    CredentialGuard is not enabled[0m
    Virtualization Based Security Status:      [0m[1;31mNot enabled[0m
    Configured:                                [0m[1;31mFalse[0m
    Running:                                   [0m[1;31mFalse[0m

[1;36m╔══════════╣ [1;32mCached Creds[0m
[1;36m╚ [1;34mIf > 0, credentials will be cached in the registry and accessible by SYSTEM user [1;33mhttps://book.hacktricks.xyz/windows-hardening/stealing-credentials/credentials-protections#cached-credentials[0m
[1;31m    cachedlogonscount is 10[0m

[1;36m╔══════════╣ [1;32mEnumerating saved credentials in Registry (CurrentPass)[0m

[1;36m╔══════════╣ [1;32mAV Information[0m
[1;32m    Some AV was detected, search for bypasses[0m
[1;37m    Name: [0mWindows Defender
[1;37m    ProductEXE: [0mwindowsdefender://
[1;37m    pathToSignedReportingExe: [0m%ProgramFiles%\Windows Defender\MsMpeng.exe

[1;36m╔══════════╣ [1;32mWindows Defender configuration[0m

[1;36m╔══════════╣ [1;32mUAC Status[0m
[1;36m╚ [1;34mIf you are in the Administrators group check how to bypass the UAC [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#basic-uac-bypass-full-file-system-access[0m
[1;37m    ConsentPromptBehaviorAdmin: [0m5 - [0m[1;31mPromptForNonWindowsBinaries[0m
[1;37m    EnableLUA: [0m1
[1;37m    LocalAccountTokenFilterPolicy: [0m
[1;37m    FilterAdministratorToken: [0m
[1;32m      [*] LocalAccountTokenFilterPolicy set to 0 and FilterAdministratorToken != 1.
      [-] Only the RID-500 local admin account can be used for lateral movement.[0m

[1;36m╔══════════╣ [1;32mPowerShell Settings[0m
[1;37m    PowerShell v2 Version: [0m2.0
[1;37m    PowerShell v5 Version: [0m5.1.22000.1
[1;37m    PowerShell Core Version: [0m
[1;37m    Transcription Settings: [0m
[1;37m    Module Logging Settings: [0m
[1;37m    Scriptblock Logging Settings: [0m
[1;37m    [0m[1;31mPS history file: [0mC:\Users\alex\AppData\Roaming\Microsoft\Windows\PowerShell\PSReadLine\ConsoleHost_history.txt[0m
[1;37m    [0m[1;31mPS history size: [0m383B[0m

[1;36m╔══════════╣ [1;32mEnumerating PowerShell Session Settings using the registry[0m
      You must be an administrator to run this check

[1;36m╔══════════╣ [1;32mPS default transcripts history[0m
[1;36m╚ [1;34mRead the PS history inside these files (if any)[0m

[1;36m╔══════════╣ [1;32mHKCU Internet Settings[0m
[1;37m    CertificateRevocation: [0m1
[1;37m    DisableCachingOfSSLPages: [0m0
[1;37m    IE5_UA_Backup_Flag: [0m5.0
[1;37m    PrivacyAdvanced: [0m1
[1;37m    SecureProtocols: [0m10240
[1;37m    User Agent: [0mMozilla/4.0 (compatible; MSIE 8.0; Win32)
[1;37m    ZonesSecurityUpgrade: [0mSystem.Byte[]
[1;37m    WarnonZoneCrossing: [0m0
[1;37m    EnableNegotiate: [0m1
[1;37m    ProxyEnable: [0m0
[1;37m    MigrateProxy: [0m1

[1;36m╔══════════╣ [1;32mHKLM Internet Settings[0m
[1;37m    ActiveXCache: [0mC:\Windows\Downloaded Program Files
[1;37m    CodeBaseSearchPath: [0mCODEBASE
[1;37m    EnablePunycode: [0m1
[1;37m    MinorVersion: [0m0
[1;37m    WarnOnIntranet: [0m1

[1;36m╔══════════╣ [1;32mDrives Information[0m
[1;36m╚ [1;34mRemember that you should search more info inside the other drives [1;33m[0m
    C:\ (Type: Fixed)(Filesystem: NTFS)(Available space: 3 GB)([0m[1;31mPermissions: Authenticated Users [AppendData/CreateDirectories])[0m
    D:\ (Type: CDRom)

[1;36m╔══════════╣ [1;32mChecking WSUS[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#wsus[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mChecking KrbRelayUp[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#krbrelayup[0m
[1;32m  The system isn't inside a domain, so it isn't vulnerable[0m

[1;36m╔══════════╣ [1;32mChecking If Inside Container[0m
[1;36m╚ [1;34mIf the binary cexecsvc.exe or associated service exists, you are inside Docker [1;33m[0m
[1;32mYou are NOT inside a container[0m

[1;36m╔══════════╣ [1;32mChecking AlwaysInstallElevated[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#alwaysinstallelevated[0m
[1;32m    AlwaysInstallElevated isn't available[0m

[1;36m╔══════════╣ [1;32mEnumerate LSA settings - auth packages included
[0m
    auditbasedirectories                 :       0
    auditbaseobjects                     :       0
    Authentication Packages              :       msv1_0
    Bounds                               :       00-30-00-00-00-20-00-00
    crashonauditfail                     :       0
    fullprivilegeauditing                :       00
    LimitBlankPasswordUse                :       1
    NoLmHash                             :       1
    Notification Packages                :       scecli
    Security Packages                    :       ""
    LsaPid                               :       708
    LsaCfgFlagsDefault                   :       0
    SecureBoot                           :       1
    ProductType                          :       6
    disabledomaincreds                   :       0
    everyoneincludesanonymous            :       0
    forceguest                           :       0
    restrictanonymous                    :       0
    restrictanonymoussam                 :       1

[1;36m╔══════════╣ [1;32mEnumerating NTLM Settings[0m
[1;31m  LanmanCompatibilityLevel    :  (Send NTLMv2 response only - Win7+ default)
[0m
[1;34m
  NTLM Signing Settings[0m
      ClientRequireSigning    : [0m[1;31mFalse[0m
      ClientNegotiateSigning  : [0m[1;32mTrue[0m
      ServerRequireSigning    : [0m[1;31mFalse[0m
      ServerNegotiateSigning  : [0m[1;31mFalse[0m
      LdapSigning             : [0m[33m[0m[33mNegotiate signing[0m[0m ([0m[33m[0m[33mNegotiate signing[0m[0m)
[1;34m
  Session Security[0m
[1;32m      NTLMMinClientSec        : 536870912 (Require 128-bit encryption)[0m
[1;32m      NTLMMinServerSec        : 536870912 (Require 128-bit encryption)
[0m
[1;34m
  NTLM Auditing and Restrictions[0m
      InboundRestrictions     :  (Not defined)
[1;31m      OutboundRestrictions    :  (Not defined)[0m
      InboundAuditing         :  (Not defined)
      OutboundExceptions      : 

[1;36m╔══════════╣ [1;32mDisplay Local Group Policy settings - local users/machine[0m

[1;36m╔══════════╣ [1;32mChecking AppLocker effective policy[0m
   AppLockerPolicy version: 1
   listing rules:



[1;36m╔══════════╣ [1;32mEnumerating Printers (WMI)[0m

[1;36m╔══════════╣ [1;32mEnumerating Named Pipes[0m
  Name                                                                                                 CurrentUserPerms                                                       Sddl

  eventlog                                                                                             [0m[1;31mEveryone [WriteData/CreateFiles][0m                                       O:LSG:LSD:P(A;;0x12019b;;;WD)(A;;CC;;;OW)(A;;0x12008f;;;S-1-5-80-880578595-1860270145-482643319-2788375705-1540778122)

  LOCAL\mojo.external_task_manager_1572                                                                                                                                       O:S-1-5-21-3557295818-2536705713-589665162-1003G:S-1-5-21-3557295818-2536705713-589665162-513D:(A;;FA;;;OW)(A;;FA;;;SY)(A;;FA;;;BA)

  LOCAL\S-1-5-5-0-4907790-Teams-2.0-instance-pipe                                                      [0m[1;31malex [AllAccess][0m                                                       O:S-1-5-21-3557295818-2536705713-589665162-1003G:S-1-5-21-3557295818-2536705713-589665162-513D:(A;;FR;;;WD)(A;;FR;;;AN)(A;;FA;;;SY)(A;;FA;;;BA)(A;;FA;;;S-1-5-21-3557295818-2536705713-589665162-1003)

  ProtectedPrefix\LocalService\FTHPIPE                                                                 [0m[1;31mInteractive [WriteData/CreateFiles][0m                                    O:LSG:LSD:P(A;;0x12019f;;;IU)(A;;FA;;;LS)

  SearchTextHarvester                                                                                                                                                         O:SYG:SYD:P(D;;FA;;;NU)(D;;FA;;;BG)(A;;FR;;;IU)(A;;FA;;;SY)(A;;FA;;;BA)

  vgauth-service                                                                                       [0m[1;31mEveryone [WriteData/CreateFiles][0m                                       O:BAG:SYD:P(A;;0x12019f;;;WD)(A;;FA;;;SY)(A;;FA;;;BA)


[1;36m╔══════════╣ [1;32mEnumerating AMSI registered providers[0m
    Provider:       {2781761E-28E0-4109-99FE-B9D127C57AFE}
    Path:           "C:\ProgramData\Microsoft\Windows Defender\Platform\4.18.24070.5-0\MpOav.dll"

[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mEnumerating Sysmon configuration[0m
      You must be an administrator to run this check

[1;36m╔══════════╣ [1;32mEnumerating Sysmon process creation logs (1)[0m
      You must be an administrator to run this check

[1;36m╔══════════╣ [1;32mInstalled .NET versions
[0m
[1;34m  CLR Versions[0m
   4.0.30319
[1;34m
  .NET Versions[0m
   4.8.04161
[1;34m
  .NET & AMSI (Anti-Malware Scan Interface) support[0m
      .NET version supports AMSI     : [0m[1;32mTrue[0m
      OS supports AMSI               : [0m[1;32mTrue[0m
        [!] The highest .NET version is enrolled in AMSI!


[1;36m════════════════════════════════════╣ [1;32mInteresting Events information[1;36m ╠════════════════════════════════════[0m

[1;36m╔══════════╣ [1;32mPrinting Explicit Credential Events (4648) for last 30 days - A process logged on using plaintext credentials
[0m
      You must be an administrator to run this check

[1;36m╔══════════╣ [1;32mPrinting Account Logon Events (4624) for the last 10 days.
[0m
      You must be an administrator to run this check

[1;36m╔══════════╣ [1;32mProcess creation events - searching logs (EID 4688) for sensitive data.
[0m
      You must be an administrator to run this check

[1;36m╔══════════╣ [1;32mPowerShell events - script block logs (EID 4104) - searching for sensitive data.
[0m
   User Id         :        S-1-5-21-3557295818-2536705713-589665162-1001
   Event Id        :        4104
   Context         :        Write-Output "[~] SetLocalAdminPassword: Setting password for $Username..."
$AdminUser | Enable-LocalUser
$AdminUser = Get-LocalUser -Name $Username
ConvertTo-SecureString -AsPlainText -Force
$AdminUser | Set-LocalUser -Password $SecurePassword
Write-Output "[~] SetLocalAdminPassword: Re-applying PasswordComplexity requirements..."
secedit /configure /db c:\windows\security\local.sdb /cfg c:\secpol.cfg /areas SECURITYPOLICY
   Created At      :        9/16/2022 11:03:35 AM
   Command line    :        ConvertTo-SecureString -AsPlainText -Force


[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mDisplaying Power off/on events for last 5 days
[0m


[1;36m════════════════════════════════════╣ [1;32mUsers Information[1;36m ╠════════════════════════════════════[0m

[1;36m╔══════════╣ [1;32mUsers[0m
[1;36m╚ [1;34mCheck if you have some admin equivalent privileges [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#users-and-groups[0m
  Current user: [0m[36m[0m[1;35malex[0m[0m
  Current groups: Domain Users, Everyone, Builtin\[0m[1;31m[0m[1;31m[0m[1;31mRemote [0m[0m[0mDesktop Users, Builtin\[0m[1;31m[0m[1;31m[0m[1;31mRemote [0m[0m[0mManagement Users, Users, [0m[1;31m[0m[1;31m[0m[1;31mRemote [0m[0m[0mInteractive Logon, Interactive, Authenticated Users, This Organization, Local account, Local, NTLM Authentication
[1;90m   =================================================================================================[0m

    [0m[1;35mCLIENTWK222[0m\[0m[1;31mAdministrator[0m: Built-in account for administering the computer/domain
        |->Groups: [0m[1;31mAdministrator[0ms
        |->Password: CanChange-[0m[1;31mNotExpi[0m-Req

    [0m[1;35mCLIENTWK222[0m\[0m[36m[0m[1;35malex[0m[0m
        |->Groups: [0m[1;31m[0m[1;31mRemote [0m[0mDesktop Users,[0m[1;31m[0m[1;31mRemote [0m[0mManagement Users,Users
        |->Password: CanChange-[0m[1;31mNotExpi[0m-NotReq

    [0m[1;35mCLIENTWK222[0m\[0m[34mDefaultAccount[0m([0m[34mDisabled[0m): A user account managed by the system.
        |->Groups: System Managed Accounts Group
        |->Password: CanChange-[0m[1;31mNotExpi[0m-NotReq

    [0m[1;35mCLIENTWK222[0m\[0m[36mdiana[0m
        |->Groups: Performance Log Users,Users
        |->Password: CanChange-[0m[1;31mNotExpi[0m-NotReq

    [0m[1;35mCLIENTWK222[0m\[0m[36m[0m[1;31menterpriseadmin[0m[0m
        |->Groups: [0m[1;31mAdministrator[0ms,Users
        |->Password: CanChange-[0m[1;31mNotExpi[0m-NotReq

    [0m[1;35mCLIENTWK222[0m\[0m[36menterpriseuser[0m
        |->Groups: Backup Operators,Users
        |->Password: CanChange-[0m[1;31mNotExpi[0m-NotReq

    [0m[1;35mCLIENTWK222[0m\[0m[34mGuest[0m([0m[34mDisabled[0m): Built-in account for guest access to the computer/domain
        |->Groups: [0m[34mGuest[0ms
        |->Password: [0m[1;31mNotChange[0m-[0m[1;31mNotExpi[0m-NotReq

    [0m[1;35mCLIENTWK222[0m\[0m[36m[0m[1;31moffsec[0m[0m
        |->Groups: [0m[1;31mAdministrator[0ms,Users
        |->Password: CanChange-[0m[1;31mNotExpi[0m-Req

    [0m[1;35mCLIENTWK222[0m\[0m[34mWDAGUtilityAccount[0m([0m[34mDisabled[0m): A user account managed and used by the system for Windows Defender Application Guard scenarios.
        |->Password: CanChange-Expi-Req


[1;36m╔══════════╣ [1;32mCurrent User Idle Time[0m
   Current User   :     CLIENTWK222\alex
   Idle Time      :     00h:00m:00s:891ms

[1;36m╔══════════╣ [1;32mDisplay Tenant information (DsRegCmd.exe /status)[0m
   Tenant is NOT Azure AD Joined.

[1;36m╔══════════╣ [1;32mCurrent Token privileges[0m
[1;36m╚ [1;34mCheck if you can escalate privilege using some enabled token [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#token-manipulation[0m
[1;37m    SeChangeNotifyPrivilege: [0mSE_PRIVILEGE_ENABLED_BY_DEFAULT, SE_PRIVILEGE_ENABLED
[1;37m    SeUndockPrivilege: [0mDISABLED
[1;37m    SeIncreaseWorkingSetPrivilege: [0mDISABLED
[1;37m    SeTimeZonePrivilege: [0mDISABLED

[1;36m╔══════════╣ [1;32mClipboard text[0m
[1;31mGet-ItemProperty "HKLM:\SOFTWARE\Wow6432Node\Microsoft\Windows\CurrentVersion\Uninstall\*" | select displayname[0m

[1;36m╔══════════╣ [1;32mLogged users[0m
    [0m[1;35mCLIENTWK222[0m\[0m[36menterpriseuser[0m
    [0m[1;35mCLIENTWK222[0m\[0m[36m[0m[1;35malex[0m[0m
    [0m[1;35mCLIENTWK222[0m\[0m[36mdiana[0m

[1;36m╔══════════╣ [1;32mDisplay information about local users[0m
   Computer Name           :   CLIENTWK222
   User Name               :   [0m[1;31mAdministrator[0m
   User Id                 :   500
   Is Enabled              :   [0m[1;31mTrue[0m
   User Type               :   [0m[1;31mAdministrator[0m
   Comment                 :   Built-in account for administering the computer/domain
   Last Logon              :   12/6/2024 6:33:01 AM
   Logons Count            :   27
   Password Last Set       :   9/16/2022 10:04:08 AM

[1;90m   =================================================================================================[0m

   Computer Name           :   CLIENTWK222
   User Name               :   alex
   User Id                 :   1003
   Is Enabled              :   [0m[1;31mTrue[0m
   User Type               :   User
   Comment                 :   
   Last Logon              :   12/6/2024 7:55:58 AM
   Logons Count            :   8
   Password Last Set       :   9/16/2022 10:04:26 AM

[1;90m   =================================================================================================[0m

   Computer Name           :   CLIENTWK222
   User Name               :   DefaultAccount
   User Id                 :   503
   Is Enabled              :   [0m[1;32mFalse[0m
   User Type               :   [0m[33mGuest[0m
   Comment                 :   A user account managed by the system.
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

[1;90m   =================================================================================================[0m

   Computer Name           :   CLIENTWK222
   User Name               :   diana
   User Id                 :   1002
   Is Enabled              :   [0m[1;31mTrue[0m
   User Type               :   User
   Comment                 :   
   Last Logon              :   12/6/2024 8:15:42 AM
   Logons Count            :   142
   Password Last Set       :   9/16/2022 10:04:20 AM

[1;90m   =================================================================================================[0m

   Computer Name           :   CLIENTWK222
   User Name               :   enterpriseadmin
   User Id                 :   1001
   Is Enabled              :   [0m[1;31mTrue[0m
   User Type               :   [0m[1;31mAdministrator[0m
   Comment                 :   
   Last Logon              :   9/21/2022 2:48:03 PM
   Logons Count            :   16
   Password Last Set       :   9/16/2022 10:04:36 AM

[1;90m   =================================================================================================[0m

   Computer Name           :   CLIENTWK222
   User Name               :   enterpriseuser
   User Id                 :   1004
   Is Enabled              :   [0m[1;31mTrue[0m
   User Type               :   User
   Comment                 :   
   Last Logon              :   10/3/2024 9:34:59 AM
   Logons Count            :   18
   Password Last Set       :   9/16/2022 10:04:31 AM

[1;90m   =================================================================================================[0m

   Computer Name           :   CLIENTWK222
   User Name               :   [0m[33mGuest[0m
   User Id                 :   501
   Is Enabled              :   [0m[1;32mFalse[0m
   User Type               :   [0m[33mGuest[0m
   Comment                 :   Built-in account for guest access to the computer/domain
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   1/1/1970 12:00:00 AM

[1;90m   =================================================================================================[0m

   Computer Name           :   CLIENTWK222
   User Name               :   offsec
   User Id                 :   1005
   Is Enabled              :   [0m[1;31mTrue[0m
   User Type               :   [0m[1;31mAdministrator[0m
   Comment                 :   
   Last Logon              :   12/6/2024 6:33:09 AM
   Logons Count            :   13
   Password Last Set       :   11/15/2022 11:06:46 AM

[1;90m   =================================================================================================[0m

   Computer Name           :   CLIENTWK222
   User Name               :   WDAGUtilityAccount
   User Id                 :   504
   Is Enabled              :   [0m[1;32mFalse[0m
   User Type               :   [0m[33mGuest[0m
   Comment                 :   A user account managed and used by the system for Windows Defender Application Guard scenarios.
   Last Logon              :   1/1/1970 12:00:00 AM
   Logons Count            :   0
   Password Last Set       :   9/15/2022 8:27:25 PM

[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mRDP Sessions[0m
[1;90m    SessID    pSessionName   pUserName      pDomainName              State     SourceIP[0m
    2         RDP-Tcp#0      [0m[36m[0m[1;35malex[0m[0m           [0m[1;35mCLIENTWK222[0m              Active    192.168.45.213

[1;36m╔══════════╣ [1;32mEver logged users[0m
    [0m[1;35mCLIENTWK222[0m\[0m[1;31mAdministrator[0m
    [0m[1;35mCLIENTWK222[0m\[0m[36m[0m[1;31moffsec[0m[0m
    [0m[1;35mCLIENTWK222[0m\[0m[36menterpriseuser[0m
    [0m[1;35mCLIENTWK222[0m\[0m[36m[0m[1;35malex[0m[0m
    [0m[1;35mCLIENTWK222[0m\[0m[36mdiana[0m
    [0m[1;35mCLIENTWK222[0m\[0m[36m[0m[1;31menterpriseadmin[0m[0m

[1;36m╔══════════╣ [1;32mHome folders found[0m
[1;32m    C:\Users\Administrator[0m
[1;31m    C:\Users\alex : alex [AllAccess][0m
[1;32m    C:\Users\All Users[0m
[1;32m    C:\Users\Default[0m
[1;32m    C:\Users\Default User[0m
[1;32m    C:\Users\diana[0m
[1;32m    C:\Users\enterpriseadmin[0m
[1;32m    C:\Users\enterpriseuser[0m
[1;32m    C:\Users\offsec[0m
[1;31m    C:\Users\Public : Interactive [WriteData/CreateFiles][0m

[1;36m╔══════════╣ [1;32mLooking for AutoLogon credentials[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mPassword Policies[0m
[1;36m╚ [1;34mCheck for a possible brute-force [1;33m[0m
[1;37m    Domain: [0mBuiltin
[1;37m    SID: [0mS-1-5-32
[1;37m    MaxPasswordAge: [0m42.22:47:31.7437440
[1;37m    MinPasswordAge: [0m00:00:00
[1;37m    MinPasswordLength: [0m0
[1;37m    PasswordHistoryLength: [0m0
[1;37m    PasswordProperties: [0m0
[1;90m   =================================================================================================[0m

[1;37m    Domain: [0m[0m[1;35mCLIENTWK222[0m
[1;37m    SID: [0mS-1-5-21-3557295818-2536705713-589665162
[1;37m    MaxPasswordAge: [0m42.00:00:00
[1;37m    MinPasswordAge: [0m00:00:00
[1;37m    MinPasswordLength: [0m0
[1;37m    PasswordHistoryLength: [0m0
[1;37m    PasswordProperties: [0m0
[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mPrint Logon Sessions[0m
    Method:                       WMI
    Logon Server:                 
    Logon Server Dns Domain:      
    Logon Id:                     4907917
    Logon Time:                   
    Logon Type:                   RemoteInteractive
    Start Time:                   12/6/2024 7:55:58 AM
    Domain:                       CLIENTWK222
    Authentication Package:       NTLM
    Start Time:                   12/6/2024 7:55:58 AM
    User Name:                    alex
    User Principal Name:          
    User SID:                     

[1;90m   =================================================================================================[0m

    Method:                       WMI
    Logon Server:                 
    Logon Server Dns Domain:      
    Logon Id:                     4885006
    Logon Time:                   
    Logon Type:                   Network
    Start Time:                   12/6/2024 7:55:56 AM
    Domain:                       CLIENTWK222
    Authentication Package:       NTLM
    Start Time:                   12/6/2024 7:55:56 AM
    User Name:                    alex
    User Principal Name:          
    User SID:                     

[1;90m   =================================================================================================[0m



[1;36m════════════════════════════════════╣ [1;32mProcesses Information[1;36m ╠════════════════════════════════════[0m

[1;36m╔══════════╣ [1;32mInteresting Processes -non Microsoft-[0m
[1;36m╚ [1;34mCheck if any interesting processes for memory dump or if you could overwrite some binary running [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#running-processes[0m
    cmd(1976)[[0m[1;32mC:\Windows\system32\cmd.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Windows\system32\cmd.exe" 
[1;90m   =================================================================================================[0m

    ShellExperienceHost(9472)[[0m[1;32mC:\Windows\SystemApps\ShellExperienceHost_cw5n1h2txyewy\ShellExperienceHost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Windows\SystemApps\ShellExperienceHost_cw5n1h2txyewy\ShellExperienceHost.exe" -ServerName:App.AppXtk181tbxbce2qsex02s8tw7hfxa9xb3t.mca
[1;90m   =================================================================================================[0m

    sihost(6884)[[0m[1;32mC:\Windows\system32\sihost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: sihost.exe
[1;90m   =================================================================================================[0m

    msedgewebview2(8600)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --type=renderer --noerrdialogs --user-data-dir="C:\Users\alex\AppData\Local\Packages\MicrosoftTeams_8wekyb3d8bbwe\LocalCache\Microsoft\MSTeams\EBWebView" --webview-exe-name=msteams.exe --webview-exe-version=24215.1105.3082.1600 --embedded-browser-webview=1 --embedded-browser-webview-dpi-awareness=2 --autoplay-policy=no-user-gesture-required --video-capture-use-gpu-memory-buffer --lang=en-US --device-scale-factor=1 --num-raster-threads=1 --renderer-client-id=5 --js-flags="--harmony-weak-refs-with-cleanup-some --expose-gc --ms-user-locale=" --time-ticks-at-unix-epoch=-1733495428402214 --launch-time-ticks=5151296503 --field-trial-handle=3484,i,14369151086299492479,926037904162180670,262144 --enable-features=AutofillReplaceCachedWebElementsByRendererIds,MojoIpcz,msAbydos,msAbydosGestureSupport,msAbydosHandwritingAttr,msSingleSignOnOSForPrimaryAccountIsShared,msWebView2EnableDraggableRegions,msWebView2SetUserAgentOverrideOnIframes --disable-features=BreakoutBoxPreferCaptureTimestampInVideoFrames,V8Maglev,msFloatyShouldHonorIndiaHoldout,msWebOOUI --variations-seed-version --mojo-platform-channel-handle=3500 /prefetch:1
[1;90m   =================================================================================================[0m

    msedgewebview2(8288)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --type=crashpad-handler --user-data-dir=C:\Users\alex\AppData\Local\Packages\MicrosoftTeams_8wekyb3d8bbwe\LocalCache\Microsoft\MSTeams\EBWebView /prefetch:4 --monitor-self-annotation=ptype=crashpad-handler --database=C:\Users\alex\AppData\Local\Packages\MicrosoftTeams_8wekyb3d8bbwe\LocalCache\Microsoft\MSTeams\EBWebView\Crashpad --annotation=IsOfficialBuild=1 --annotation=channel= --annotation=chromium-version=128.0.6613.114 "--annotation=exe=C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --annotation=plat=Win64 "--annotation=prod=Edge WebView2" --annotation=ver=128.0.2739.54 --initial-client-data=0x164,0x168,0x16c,0x140,0x11c,0x7fff58f49fd8,0x7fff58f49fe4,0x7fff58f49ff0
[1;90m   =================================================================================================[0m

    SearchHost(4660)[[0m[1;32mC:\Windows\SystemApps\MicrosoftWindows.Client.CBS_cw5n1h2txyewy\SearchHost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Windows\SystemApps\MicrosoftWindows.Client.CBS_cw5n1h2txyewy\SearchHost.exe" -ServerName:CortanaUI.AppXstmwaab17q5s3y22tp6apqz7a45vwv65.mca
[1;90m   =================================================================================================[0m

    RuntimeBroker(4276)[[0m[1;32mC:\Windows\System32\RuntimeBroker.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\System32\RuntimeBroker.exe [0m-Embedding
[1;90m   =================================================================================================[0m

    msedgewebview2(8572)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --type=utility --utility-sub-type=storage.mojom.StorageService --lang=en-US --service-sandbox-type=service --noerrdialogs --user-data-dir="C:\Users\alex\AppData\Local\Packages\MicrosoftTeams_8wekyb3d8bbwe\LocalCache\Microsoft\MSTeams\EBWebView" --webview-exe-name=msteams.exe --webview-exe-version=24215.1105.3082.1600 --embedded-browser-webview=1 --embedded-browser-webview-dpi-awareness=2 --field-trial-handle=1712,i,14369151086299492479,926037904162180670,262144 --enable-features=AutofillReplaceCachedWebElementsByRendererIds,MojoIpcz,msAbydos,msAbydosGestureSupport,msAbydosHandwritingAttr,msSingleSignOnOSForPrimaryAccountIsShared,msWebView2EnableDraggableRegions,msWebView2SetUserAgentOverrideOnIframes --disable-features=BreakoutBoxPreferCaptureTimestampInVideoFrames,V8Maglev,msFloatyShouldHonorIndiaHoldout,msWebOOUI --variations-seed-version --mojo-platform-channel-handle=2316 /prefetch:13
[1;90m   =================================================================================================[0m

    msedge(1572)[[0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --no-startup-window
[1;90m   =================================================================================================[0m

    dllhost(7708)[[0m[1;32mC:\Windows\system32\DllHost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\system32\DllHost.exe [0m/Processid:{AB8902B4-09CA-4BB6-B78D-A8F59079A8D5}
[1;90m   =================================================================================================[0m

    taskhostw(804)[[0m[1;32mC:\Windows\system32\taskhostw.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: taskhostw.exe {222A245B-E637-4AE9-A93F-A59CA119A75E}
[1;90m   =================================================================================================[0m

    Widgets(3388)[[0m[1;32mC:\Program Files\WindowsApps\MicrosoftWindows.Client.WebExperience_421.20070.765.0_x64__cw5n1h2txyewy\Dashboard\Widgets.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files\WindowsApps\MicrosoftWindows.Client.WebExperience_421.20070.765.0_x64__cw5n1h2txyewy\Dashboard\Widgets.exe" -ServerName:Microsoft.Windows.DashboardServer
[1;90m   =================================================================================================[0m

    svchost(5092)[[0m[1;32mC:\Windows\system32\svchost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\system32\svchost.exe [0m-k ClipboardSvcGroup -p -s cbdhsvc
[1;90m   =================================================================================================[0m

    SecurityHealthSystray(8108)[[0m[1;32mC:\Windows\System32\SecurityHealthSystray.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Windows\System32\SecurityHealthSystray.exe" 
[1;90m   =================================================================================================[0m

    msedgewebview2(7656)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --type=renderer --noerrdialogs --user-data-dir="C:\Users\alex\AppData\Local\Packages\MicrosoftWindows.Client.WebExperience_cw5n1h2txyewy\LocalState\EBWebView" --webview-exe-name=Widgets.exe --webview-exe-version=421.20070.825.0 --embedded-browser-webview=1 --embedded-browser-webview-dpi-awareness=2 --video-capture-use-gpu-memory-buffer --lang=en-US --device-scale-factor=1 --num-raster-threads=1 --renderer-client-id=5 --js-flags="--harmony-weak-refs-with-cleanup-some --expose-gc --ms-user-locale=" --time-ticks-at-unix-epoch=-1733495428404681 --launch-time-ticks=6035772635 --field-trial-handle=3468,i,306851916249040945,342587212730388463,262144 --enable-features=MojoIpcz,UseBackgroundNativeThreadPool,UseNativeThreadPool,msWebView2TreatAppSuspendAsDeviceSuspend --variations-seed-version --mojo-platform-channel-handle=1588 /prefetch:1
[1;90m   =================================================================================================[0m

    msteams(7224)[[0m[1;32mC:\Program Files\WindowsApps\MicrosoftTeams_24215.1105.3082.1600_x64__8wekyb3d8bbwe\msteams.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files\WindowsApps\MicrosoftTeams_24215.1105.3082.1600_x64__8wekyb3d8bbwe\msteams.exe" ms-teams:system-initiated
[1;90m   =================================================================================================[0m

    msedge(5920)[[0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --type=crashpad-handler "--user-data-dir=C:\Users\alex\AppData\Local\Microsoft\Edge\User Data" /prefetch:4 --monitor-self-annotation=ptype=crashpad-handler "--database=C:\Users\alex\AppData\Local\Microsoft\Edge\User Data\Crashpad" --annotation=IsOfficialBuild=1 --annotation=channel= --annotation=chromium-version=128.0.6613.114 "--annotation=exe=C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --annotation=plat=Win64 --annotation=prod=Edge --annotation=ver=128.0.2739.54 --initial-client-data=0x258,0x25c,0x260,0x254,0x268,0x7fff58f49fd8,0x7fff58f49fe4,0x7fff58f49ff0
[1;90m   =================================================================================================[0m

    msedgewebview2(4620)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --type=crashpad-handler --user-data-dir=C:\Users\alex\AppData\Local\Packages\MicrosoftWindows.Client.WebExperience_cw5n1h2txyewy\LocalState\EBWebView /prefetch:4 --monitor-self-annotation=ptype=crashpad-handler --database=C:\Users\alex\AppData\Local\Packages\MicrosoftWindows.Client.WebExperience_cw5n1h2txyewy\LocalState\EBWebView\Crashpad --annotation=IsOfficialBuild=1 --annotation=channel= --annotation=chromium-version=128.0.6613.114 "--annotation=exe=C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --annotation=plat=Win64 "--annotation=prod=Edge WebView2" --annotation=ver=128.0.2739.54 --initial-client-data=0x164,0x168,0x16c,0x140,0x1a0,0x7fff58f49fd8,0x7fff58f49fe4,0x7fff58f49ff0
[1;90m   =================================================================================================[0m

    OneDrive(2456)[[0m[1;31mC:\Users\alex\AppData\Local\Microsoft\OneDrive\OneDrive.exe][0m -- POwn:[0m[1;35m alex[0m
    [0m[1;31mPermissions:[0m[1;35m alex[0m [AllAccess][0m
    [0m[1;31mPossible DLL Hijacking folder: C:\Users\alex\AppData\Local\Microsoft\OneDrive (alex [AllAccess])[0m
    [1;37mCommand Line: "C:\Users\alex\AppData\Local\Microsoft\OneDrive\OneDrive.exe" /background
[1;90m   =================================================================================================[0m

    msedgewebview2(8468)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --type=utility --utility-sub-type=network.mojom.NetworkService --lang=en-US --service-sandbox-type=none --noerrdialogs --user-data-dir="C:\Users\alex\AppData\Local\Packages\MicrosoftTeams_8wekyb3d8bbwe\LocalCache\Microsoft\MSTeams\EBWebView" --webview-exe-name=msteams.exe --webview-exe-version=24215.1105.3082.1600 --embedded-browser-webview=1 --embedded-browser-webview-dpi-awareness=2 --field-trial-handle=2044,i,14369151086299492479,926037904162180670,262144 --enable-features=AutofillReplaceCachedWebElementsByRendererIds,MojoIpcz,msAbydos,msAbydosGestureSupport,msAbydosHandwritingAttr,msSingleSignOnOSForPrimaryAccountIsShared,msWebView2EnableDraggableRegions,msWebView2SetUserAgentOverrideOnIframes --disable-features=BreakoutBoxPreferCaptureTimestampInVideoFrames,V8Maglev,msFloatyShouldHonorIndiaHoldout,msWebOOUI --variations-seed-version --mojo-platform-channel-handle=2052 /prefetch:11
[1;90m   =================================================================================================[0m

    StartMenuExperienceHost(5012)[[0m[1;32mC:\Windows\SystemApps\Microsoft.Windows.StartMenuExperienceHost_cw5n1h2txyewy\StartMenuExperienceHost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Windows\SystemApps\Microsoft.Windows.StartMenuExperienceHost_cw5n1h2txyewy\StartMenuExperienceHost.exe" -ServerName:App.AppXywbrabmsek0gm3tkwpr5kwzbs55tkqay.mca
[1;90m   =================================================================================================[0m

    msedgewebview2(8456)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --type=gpu-process --noerrdialogs --user-data-dir="C:\Users\alex\AppData\Local\Packages\MicrosoftTeams_8wekyb3d8bbwe\LocalCache\Microsoft\MSTeams\EBWebView" --webview-exe-name=msteams.exe --webview-exe-version=24215.1105.3082.1600 --embedded-browser-webview=1 --embedded-browser-webview-dpi-awareness=2 --gpu-preferences=UAAAAAAAAADgAAAMAAAAAAAAAAAAAAAAAABgAAEAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAAAAAAAAAAEAAAAAAAAAAIAAAAAAAAAAgAAAAAAAAA --field-trial-handle=1808,i,14369151086299492479,926037904162180670,262144 --enable-features=AutofillReplaceCachedWebElementsByRendererIds,MojoIpcz,msAbydos,msAbydosGestureSupport,msAbydosHandwritingAttr,msSingleSignOnOSForPrimaryAccountIsShared,msWebView2EnableDraggableRegions,msWebView2SetUserAgentOverrideOnIframes --disable-features=BreakoutBoxPreferCaptureTimestampInVideoFrames,V8Maglev,msFloatyShouldHonorIndiaHoldout,msWebOOUI --variations-seed-version --mojo-platform-channel-handle=1616 /prefetch:2
[1;90m   =================================================================================================[0m

    svchost(6292)[[0m[1;32mC:\Windows\system32\svchost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\system32\svchost.exe [0m-k UnistackSvcGroup -s CDPUserSvc
[1;90m   =================================================================================================[0m

    svchost(7776)[[0m[1;32mC:\Windows\System32\svchost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\System32\svchost.exe [0m-k UnistackSvcGroup
[1;90m   =================================================================================================[0m

    msedgewebview2(7968)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --embedded-browser-webview=1 --webview-exe-name=Widgets.exe --webview-exe-version=421.20070.825.0 --user-data-dir="C:\Users\alex\AppData\Local\Packages\MicrosoftWindows.Client.WebExperience_cw5n1h2txyewy\LocalState\EBWebView" --noerrdialogs --embedded-browser-webview-dpi-awareness=2 --disk-cache-size=52428800 --edge-webview-is-background --enable-features=MojoIpcz,msWebView2TreatAppSuspendAsDeviceSuspend,UseNativeThreadPool,UseBackgroundNativeThreadPool --lang=en-US --mojo-named-platform-channel-pipe=3388.9180.7187531952327901843
[1;90m   =================================================================================================[0m

    msedge(10108)[[0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --type=gpu-process --gpu-preferences=UAAAAAAAAADgAAAMAAAAAAAAAAAAAAAAAABgAAEAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAAAAAAAAAAEAAAAAAAAAAIAAAAAAAAAAgAAAAAAAAA --field-trial-handle=2160,i,6319255498609297036,10897853894442322596,262144 --variations-seed-version --mojo-platform-channel-handle=2156 /prefetch:2
[1;90m   =================================================================================================[0m

    msedge(4068)[[0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --type=utility --utility-sub-type=network.mojom.NetworkService --lang=en-US --service-sandbox-type=none --field-trial-handle=1872,i,6319255498609297036,10897853894442322596,262144 --variations-seed-version --mojo-platform-channel-handle=2344 /prefetch:11
[1;90m   =================================================================================================[0m

    PhoneExperienceHost(6220)[[0m[1;32mC:\Program Files\WindowsApps\Microsoft.YourPhone_1.22092.214.0_x64__8wekyb3d8bbwe\PhoneExperienceHost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files\WindowsApps\Microsoft.YourPhone_1.22092.214.0_x64__8wekyb3d8bbwe\PhoneExperienceHost.exe" -ComServer:Background -Embedding
[1;90m   =================================================================================================[0m

    rdpclip(1904)[[0m[1;32mC:\Windows\System32\rdpclip.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: rdpclip
[1;90m   =================================================================================================[0m

    conhost(7892)[[0m[1;32mC:\Windows\system32\conhost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: \??\[0m[1;32mC:\Windows\system32\conhost.exe [0m0x4
[1;90m   =================================================================================================[0m

    powershell(7880)[[0m[1;32mC:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Windows\System32\WindowsPowerShell\v1.0\powershell.exe" 
[1;90m   =================================================================================================[0m

    msedgewebview2(7012)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --type=gpu-process --noerrdialogs --user-data-dir="C:\Users\alex\AppData\Local\Packages\MicrosoftWindows.Client.WebExperience_cw5n1h2txyewy\LocalState\EBWebView" --webview-exe-name=Widgets.exe --webview-exe-version=421.20070.825.0 --embedded-browser-webview=1 --embedded-browser-webview-dpi-awareness=2 --gpu-preferences=UAAAAAAAAADgAAAMAAAAAAAAAAAAAAAAAABgAAEAAAAAAAAABAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABAAAAAAAAAAEAAAAAAAAAAIAAAAAAAAAAgAAAAAAAAA --field-trial-handle=1820,i,306851916249040945,342587212730388463,262144 --enable-features=MojoIpcz,UseBackgroundNativeThreadPool,UseNativeThreadPool,msWebView2TreatAppSuspendAsDeviceSuspend --variations-seed-version --mojo-platform-channel-handle=1816 /prefetch:2
[1;90m   =================================================================================================[0m

    conhost(10064)[[0m[1;32mC:\Windows\system32\conhost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: \??\[0m[1;32mC:\Windows\system32\conhost.exe [0m0x4
[1;90m   =================================================================================================[0m

    MiniSearchHost(3964)[[0m[1;32mC:\Windows\SystemApps\MicrosoftWindows.Client.CBS_cw5n1h2txyewy\MiniSearchHost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Windows\SystemApps\MicrosoftWindows.Client.CBS_cw5n1h2txyewy\MiniSearchHost.exe" -ServerName:MiniSearchUI.AppXj3y73at8fy1htwztzxs68sxx1v7cksp7.mca
[1;90m   =================================================================================================[0m

    RuntimeBroker(6976)[[0m[1;32mC:\Windows\System32\RuntimeBroker.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\System32\RuntimeBroker.exe [0m-Embedding
[1;90m   =================================================================================================[0m

    msedge(4388)[[0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\Edge\Application\msedge.exe" --type=utility --utility-sub-type=storage.mojom.StorageService --lang=en-US --service-sandbox-type=service --field-trial-handle=2468,i,6319255498609297036,10897853894442322596,262144 --variations-seed-version --mojo-platform-channel-handle=2448 /prefetch:13
[1;90m   =================================================================================================[0m

    msedgewebview2(8264)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --embedded-browser-webview=1 --webview-exe-name=msteams.exe --webview-exe-version=24215.1105.3082.1600 --user-data-dir="C:\Users\alex\AppData\Local\Packages\MicrosoftTeams_8wekyb3d8bbwe\LocalCache\Microsoft\MSTeams\EBWebView" --noerrdialogs --embedded-browser-webview-dpi-awareness=2 --autoplay-policy=no-user-gesture-required --disable-features=BreakoutBoxPreferCaptureTimestampInVideoFrames,V8Maglev,msFloatyShouldHonorIndiaHoldout,msWebOOUI --enable-features=MojoIpcz,msSingleSignOnOSForPrimaryAccountIsShared,AutofillReplaceCachedWebElementsByRendererIds,msAbydos,msAbydosGestureSupport,msAbydosHandwritingAttr,msWebView2EnableDraggableRegions,msWebView2SetUserAgentOverrideOnIframes --lang=en-US --mojo-named-platform-channel-pipe=7224.8260.18339953377547496801
[1;90m   =================================================================================================[0m

    RuntimeBroker(7400)[[0m[1;32mC:\Windows\System32\RuntimeBroker.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\System32\RuntimeBroker.exe [0m-Embedding
[1;90m   =================================================================================================[0m

    RuntimeBroker(9912)[[0m[1;32mC:\Windows\System32\RuntimeBroker.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\System32\RuntimeBroker.exe [0m-Embedding
[1;90m   =================================================================================================[0m

    msedgewebview2(8252)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --type=utility --utility-sub-type=network.mojom.NetworkService --lang=en-US --service-sandbox-type=none --noerrdialogs --user-data-dir="C:\Users\alex\AppData\Local\Packages\MicrosoftWindows.Client.WebExperience_cw5n1h2txyewy\LocalState\EBWebView" --webview-exe-name=Widgets.exe --webview-exe-version=421.20070.825.0 --embedded-browser-webview=1 --embedded-browser-webview-dpi-awareness=2 --field-trial-handle=1932,i,306851916249040945,342587212730388463,262144 --enable-features=MojoIpcz,UseBackgroundNativeThreadPool,UseNativeThreadPool,msWebView2TreatAppSuspendAsDeviceSuspend --variations-seed-version --mojo-platform-channel-handle=432 /prefetch:11
[1;90m   =================================================================================================[0m

    svchost(1084)[[0m[1;32mC:\Windows\system32\svchost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\system32\svchost.exe [0m-k UnistackSvcGroup -s WpnUserService
[1;90m   =================================================================================================[0m

    explorer(6512)[[0m[1;32mC:\Windows\Explorer.EXE][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: C:\Windows\Explorer.EXE
[1;90m   =================================================================================================[0m

    dllhost(5216)[[0m[1;32mC:\Windows\system32\DllHost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\system32\DllHost.exe [0m/Processid:{973D20D7-562D-44B9-B70B-5A0F49CCDF3F}
[1;90m   =================================================================================================[0m

    winPEASany(1244)[[0m[1;31mC:\Users\alex\Desktop\winPEASany.exe][0m -- POwn:[0m[1;35m alex[0m -- isDotNet
    [0m[1;31mPermissions:[0m[1;35m alex[0m [AllAccess][0m
    [0m[1;31mPossible DLL Hijacking folder: C:\Users\alex\Desktop (alex [AllAccess])[0m
    [1;37mCommand Line: "C:\Users\alex\Desktop\winPEASany.exe"
[1;90m   =================================================================================================[0m

    svchost(5624)[[0m[1;32mC:\Windows\system32\svchost.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: [0m[1;32mC:\Windows\system32\svchost.exe [0m-k UdkSvcGroup -s UdkUserSvc
[1;90m   =================================================================================================[0m

    vmtoolsd(8124)[[0m[1;32mC:\Program Files\VMware\VMware Tools\vmtoolsd.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files\VMware\VMware Tools\vmtoolsd.exe" -n vmusr
[1;90m   =================================================================================================[0m

    msedgewebview2(6016)[[0m[1;32mC:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe][0m -- POwn:[0m[1;35m alex[0m
    [1;37mCommand Line: "C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe" --type=utility --utility-sub-type=storage.mojom.StorageService --lang=en-US --service-sandbox-type=service --noerrdialogs --user-data-dir="C:\Users\alex\AppData\Local\Packages\MicrosoftWindows.Client.WebExperience_cw5n1h2txyewy\LocalState\EBWebView" --webview-exe-name=Widgets.exe --webview-exe-version=421.20070.825.0 --embedded-browser-webview=1 --embedded-browser-webview-dpi-awareness=2 --field-trial-handle=2272,i,306851916249040945,342587212730388463,262144 --enable-features=MojoIpcz,UseBackgroundNativeThreadPool,UseNativeThreadPool,msWebView2TreatAppSuspendAsDeviceSuspend --variations-seed-version --mojo-platform-channel-handle=2532 /prefetch:13
[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mVulnerable Leaked Handlers[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation/leaked-handle-exploitation[0m
[1;36m╚ [1;34mGetting Leaked Handlers, it might take some time...[0m
[######----]  60% |8% /#---]  73% -#--]  80% \4% |7% /#-]  90% -4% \8% |                   [1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mTakeOwnership[0m
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mAllAccess
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1844(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    File Path: [0m\Windows\System32
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m1936(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectall
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2184(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\main\featurecontrol
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2188(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\policies\microsoft\windows\currentversion\internet settings
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2196(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2200(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.newitem
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2208(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\wow6432node\microsoft\windows\currentversion\run
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2228(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore\shell\windows.selectnone
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2284(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0mTakeOwnership
[1;37m    Registry: [0mHKLM\software\microsoft\internet explorer\security
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2324(file)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    File Path: [0m\Windows\System32\en-US\svchost.exe.mui
[1;37m    File Owner: [0mNT SERVICE\TrustedInstaller
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2464(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\system\controlset001\control\nls\sorting\versions
[1;90m   =================================================================================================[0m

[1;37m    Handle: [0m2528(key)
[1;37m    Handle Owner: [0mPid is 1244(winPEASany) with owner: [0m[1;31malex[0m
[1;37m    Reason: [0m[0m[1;31mAllAccess[0m
[1;37m    Registry: [0mHKLM\software\microsoft\windows\currentversion\explorer\commandstore
[1;90m   =================================================================================================[0m



[1;36m════════════════════════════════════╣ [1;32mServices Information[1;36m ╠════════════════════════════════════[0m

[1;36m╔══════════╣ [1;32mInteresting Services -non Microsoft-[0m
[1;36m╚ [1;34mCheck if you can overwrite some service binary or perform a DLL hijacking, also check for unquoted paths [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#services[0m
    EnterpriseService(Enterprise Service Checks)[[0m[1;31m"C:\Services\EnterpriseService.exe"[0m] - Auto - Running
    [0m[1;31mPossible DLL Hijacking in binary folder: C:\Services (Authenticated Users [WriteData/CreateFiles])[0m
[1;90m   =================================================================================================[0m

    ssh-agent(OpenSSH Authentication Agent)[[0m[1;32mC:\Windows\System32\OpenSSH\ssh-agent.exe[0m] - Disabled - Stopped
    [1;37mAgent to hold private keys used for public key authentication.
[1;90m   =================================================================================================[0m

    VGAuthService(VMware, Inc. - VMware Alias Manager and Ticket Service)[[0m[1;32m"C:\Program Files\VMware\VMware Tools\VMware VGAuth\VGAuthService.exe"[0m] - Auto - Running
    [1;37mAlias Manager and Ticket Service
[1;90m   =================================================================================================[0m

    vm3dservice(VMware, Inc. - VMware SVGA Helper Service)[[0m[1;32mC:\Windows\system32\vm3dservice.exe[0m] - Auto - Running
    [1;37mHelps VMware SVGA driver by collecting and conveying user mode information
[1;90m   =================================================================================================[0m

    VMTools(VMware, Inc. - VMware Tools)[[0m[1;32m"C:\Program Files\VMware\VMware Tools\vmtoolsd.exe"[0m] - Auto - Running
    [1;37mProvides support for synchronizing objects between the host and guest operating systems.
[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mModifiable Services[0m
[1;36m╚ [1;34mCheck if you can modify any service [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#services[0m
[1;31m    LOOKS LIKE YOU CAN MODIFY OR START/STOP SOME SERVICE/s:[0m
    RmSvc: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    wcncsvc: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    BcastDVRUserService_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    ConsentUxUserSvc_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    CredentialEnrollmentManagerUserSvc_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    DeviceAssociationBrokerSvc_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    DevicePickerUserSvc_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    DevicesFlowUserSvc_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    PimIndexMaintenanceSvc_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    PrintWorkflowUserSvc_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    UdkUserSvc_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    UnistoreSvc_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    UserDataSvc_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)
    WpnUserService_4b0605: GenericExecute ([0m[33mStart[0m/[0m[33mStop[0m)

[1;36m╔══════════╣ [1;32mLooking if you can modify any service registry[0m
[1;36m╚ [1;34mCheck if you can modify the registry of a service [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#services-registry-permissions[0m
[1;32m    [-] Looks like you cannot change the registry of any service...[0m

[1;36m╔══════════╣ [1;32mChecking write permissions in PATH folders (DLL Hijacking)[0m
[1;36m╚ [1;34mCheck for DLL Hijacking in PATH folders [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#dll-hijacking[0m
[1;32m    C:\Windows\system32[0m
[1;32m    C:\Windows[0m
[1;32m    C:\Windows\System32\Wbem[0m
[1;32m    C:\Windows\System32\WindowsPowerShell\v1.0\[0m
[1;32m    C:\Windows\System32\OpenSSH\[0m


[1;36m════════════════════════════════════╣ [1;32mApplications Information[1;36m ╠════════════════════════════════════[0m

[1;36m╔══════════╣ [1;32mCurrent Active Window Application[0m
[1;32m    Windows PowerShell[0m

[1;36m╔══════════╣ [1;32mInstalled Applications --Via Program Files/Uninstall registry--[0m
[1;36m╚ [1;34mCheck if you can modify installed software [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#software[0m
[1;32m    C:\Program Files\Common Files[0m
[1;32m    C:\Program Files\desktop.ini[0m
[1;32m    C:\Program Files\Internet Explorer[0m
[1;32m    C:\Program Files\Microsoft[0m
[1;32m    C:\Program Files\Microsoft Update Health Tools[0m
[1;32m    C:\Program Files\ModifiableWindowsApps[0m
[1;32m    C:\Program Files\PackageManagement[0m
[1;32m    C:\Program Files\Uninstall Information[0m
[1;32m    C:\Program Files\VMware[0m
[1;32m    C:\Program Files\Windows Defender[0m
[1;32m    C:\Program Files\Windows Defender Advanced Threat Protection[0m
[1;32m    C:\Program Files\Windows Mail[0m
[1;32m    C:\Program Files\Windows Media Player[0m
[1;32m    C:\Program Files\Windows NT[0m
[1;32m    C:\Program Files\Windows Photo Viewer[0m
[1;32m    C:\Program Files\Windows Sidebar[0m
[1;32m    C:\Program Files\WindowsApps[0m
[1;32m    C:\Program Files\WindowsPowerShell[0m


[1;36m╔══════════╣ [1;32mAutorun Applications[0m
[1;36m╚ [1;34mCheck if you can modify other users AutoRuns binaries (Note that is normal that you can modify HKCU registry and binaries indicated there) [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation/privilege-escalation-with-autorun-binaries[0m

    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows\CurrentVersion\Run[0m
    Key: SecurityHealth
    Folder: [0m[1;32mC:\Windows\system32[0m
    File: [0m[1;32mC:\Windows\system32[0m\SecurityHealthSystray.exe
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows\CurrentVersion\Run[0m
    Key: VMware User Process
    Folder: [0m[1;32mC:\Program Files\VMware\VMware Tools[0m
    File: [0m[1;32mC:\Program Files\VMware\VMware Tools[0m\vmtoolsd.exe -n vmusr ([0m[1;31mUnquoted and Space detected[0m) - C:\
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;31mHKCU\Software\Microsoft\Windows\CurrentVersion\Run[0m
    [0m[1;31mRegPerms: alex [FullControl][0m
    Key: OneDrive
    Folder: [0m[1;31mC:\Users\alex\AppData\Local\Microsoft\OneDrive[0m
    [0m[1;31mFolderPerms: alex [AllAccess][0m
    File: [0m[1;31mC:\Users\alex\AppData\Local\Microsoft\OneDrive[0m\OneDrive.exe /background
    [0m[1;31mFilePerms: alex [AllAccess][0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;31mHKCU\Software\Microsoft\Windows\CurrentVersion\Run[0m
    [0m[1;31mRegPerms: alex [FullControl][0m
    Key: MicrosoftEdgeAutoLaunch_B2E206152823CA825CAB5FC835C2FD28
    Folder: [0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application[0m
    File: [0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application[0m\msedge.exe --no-startup-window --win-session-start ([0m[1;31mUnquoted and Space detected[0m) - C:\
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows\CurrentVersion\Explorer\Shell Folders[0m
    Key: Common Startup
    Folder: [0m[1;32mC:\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows\CurrentVersion\Explorer\User Shell Folders[0m
    Key: Common Startup
    Folder: [0m[1;32mC:\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Winlogon[0m
    Key: Userinit
    Folder: [0m[1;32mC:\Windows\system32[0m
    File: [0m[1;32mC:\Windows\system32[0m\userinit.exe,
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Winlogon[0m
    Key: Shell
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mexplorer.exe[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\SYSTEM\CurrentControlSet\Control\SafeBoot[0m
    Key: AlternateShell
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mcmd.exe[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Font Drivers[0m
    Key: Adobe Type Manager
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32matmfd.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\WOW6432Node\Microsoft\Windows NT\CurrentVersion\Font Drivers[0m
    Key: Adobe Type Manager
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32matmfd.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: aux
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwdmaud.drv[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: midi
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwdmaud.drv[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: midimapper
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmidimap.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: mixer
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwdmaud.drv[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: msacm.imaadpcm
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mimaadp32.acm[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: msacm.msadpcm
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsadp32.acm[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: msacm.msg711
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsg711.acm[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: msacm.msgsm610
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsgsm32.acm[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.i420
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32miyuv_32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.iyuv
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32miyuv_32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.mrle
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsrle32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.msvc
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsvidc32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.uyvy
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsyuv.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.yuy2
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsyuv.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.yvu9
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mtsbyuv.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.yvyu
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsyuv.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: wave
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwdmaud.drv[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: wavemapper
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsacm32.drv[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: msacm.l3acm
    Folder: [0m[1;32mC:\Windows\System32[0m
    File: [0m[1;32mC:\Windows\System32[0m\l3codeca.acm
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: aux
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwdmaud.drv[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: midi
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwdmaud.drv[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: midimapper
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmidimap.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: mixer
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwdmaud.drv[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: msacm.imaadpcm
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mimaadp32.acm[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: msacm.msadpcm
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsadp32.acm[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: msacm.msg711
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsg711.acm[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: msacm.msgsm610
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsgsm32.acm[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.cvid
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32miccvid.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.i420
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32miyuv_32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.iyuv
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32miyuv_32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.mrle
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsrle32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.msvc
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsvidc32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.uyvy
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsyuv.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.yuy2
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsyuv.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.yvu9
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mtsbyuv.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: vidc.yvyu
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsyuv.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: wave
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwdmaud.drv[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: wavemapper
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mmsacm32.drv[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows NT\CurrentVersion\Drivers32[0m
    Key: msacm.l3acm
    Folder: [0m[1;32mC:\Windows\SysWOW64[0m
    File: [0m[1;32mC:\Windows\SysWOW64[0m\l3codeca.acm
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Classes\htmlfile\shell\open\command[0m
    Folder: [0m[1;32mC:\Program Files\Internet Explorer[0m
    File: [0m[1;32mC:\Program Files\Internet Explorer[0m\iexplore.exe %1 ([0m[1;31mUnquoted and Space detected[0m) - C:\
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: *kernel32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mkernel32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: _wow64cpu
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwow64cpu.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: _wowarmhw
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwowarmhw.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: _xtajit
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mxtajit.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: advapi32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32madvapi32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: clbcatq
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mclbcatq.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: combase
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mcombase.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: COMDLG32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mCOMDLG32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: coml2
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mcoml2.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: DifxApi
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mdifxapi.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: gdi32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mgdi32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: gdiplus
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mgdiplus.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: IMAGEHLP
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mIMAGEHLP.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: IMM32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mIMM32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: MSCTF
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mMSCTF.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: MSVCRT
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mMSVCRT.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: NORMALIZ
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mNORMALIZ.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: NSI
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mNSI.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: ole32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mole32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: OLEAUT32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mOLEAUT32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: PSAPI
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mPSAPI.DLL[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: rpcrt4
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mrpcrt4.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: sechost
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32msechost.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: Setupapi
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mSetupapi.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: SHCORE
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mSHCORE.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: SHELL32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mSHELL32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: SHLWAPI
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mSHLWAPI.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: user32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32muser32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: WLDAP32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mWLDAP32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: wow64
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwow64.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: wow64base
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwow64base.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: wow64con
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwow64con.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: wow64win
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mwow64win.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: WS2_32
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mWS2_32.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\System\CurrentControlSet\Control\Session Manager\KnownDlls[0m
    Key: xtajit64
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mxtajit64.dll[0m
[1;90m   =================================================================================================[0m


    RegPath: HKLM[0m[1;31m[0m[1;31m[0m[1;31m[0m[1;31m[0m[1;31m\[0m[0m[0m[0m[0mSoftware[0m[1;31m[0m[1;31m[0m[1;31m[0m[1;31m[0m[1;31m\[0m[0m[0m[0m[0mMicrosoft[0m[1;31m[0m[1;31m[0m[1;31m[0m[1;31m[0m[1;31m\[0m[0m[0m[0m[0mActive Setup[0m[1;31m[0m[1;31m[0m[1;31m[0m[1;31m[0m[1;31m\[0m[0m[0m[0m[0mInstalled Components[0m[1;31m[0m[1;31m[0m[1;31m[0m[1;31m[0m[1;31m\[0m[0m[0m[0m[0m{2C7339CF-2B09-4501-B3F3-F3508C9228ED}
    Key: StubPath
    Folder: [0m[1;31m\[0m
    [0m[1;31mFolderPerms: Authenticated Users [AppendData/CreateDirectories][0m
    File: [0m[1;32m/UserInstall[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Active Setup\Installed Components\{6BF52A52-394A-11d3-B153-00C04F79FAA6}[0m
    Key: StubPath
    Folder: [0m[1;32mC:\Windows\system32[0m
    File: [0m[1;32mC:\Windows\system32[0m\unregmp2.exe /FirstLogon
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Active Setup\Installed Components\{89820200-ECBD-11cf-8B85-00AA005B4340}[0m
    Key: StubPath
    Folder: None ([0m[1;31mPATH Injection[0m)
    File: [0m[1;32mU[0m
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Active Setup\Installed Components\{89820200-ECBD-11cf-8B85-00AA005B4383}[0m
    Key: StubPath
    Folder: [0m[1;32mC:\Windows\System32[0m
    File: [0m[1;32mC:\Windows\System32[0m\ie4uinit.exe -UserConfig
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Active Setup\Installed Components\{89B4C1CD-B018-4511-B0A1-5476DBF70820}[0m
    Key: StubPath
    Folder: [0m[1;32mC:\Windows\System32[0m
    File: [0m[1;32m[0m[1;32mC:\Windows\System32[0m[0m\Rundll32.exe [0m[1;32m[0m[1;32mC:\Windows\System32[0m[0m\mscories.dll,Install
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Active Setup\Installed Components\{9459C573-B17A-45AE-9F64-1857B5D58CEE}[0m
    Key: StubPath
    Folder: [0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\128.0.2739.54\Installer[0m
    File: [0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\128.0.2739.54\Installer[0m\setup.exe --configure-user-settings --verbose-logging --system-level --msedge --channel=stable ([0m[1;31mUnquoted and Space detected[0m) - C:\
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Active Setup\Installed Components\{6BF52A52-394A-11d3-B153-00C04F79FAA6}[0m
    Key: StubPath
    Folder: [0m[1;32mC:\Windows\system32[0m
    File: [0m[1;32mC:\Windows\system32[0m\unregmp2.exe /FirstLogon
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Active Setup\Installed Components\{89B4C1CD-B018-4511-B0A1-5476DBF70820}[0m
    Key: StubPath
    Folder: [0m[1;32mC:\Windows\SysWOW64[0m
    File: [0m[1;32m[0m[1;32mC:\Windows\SysWOW64[0m[0m\Rundll32.exe [0m[1;32m[0m[1;32mC:\Windows\SysWOW64[0m[0m\mscories.dll,Install
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Microsoft\Windows\CurrentVersion\Explorer\Browser Helper Objects\{1FD49718-1D00-4B19-AF5F-070AF6D5D54C}[0m
    Folder: [0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\128.0.2739.54\BHO[0m
    File: [0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\128.0.2739.54\BHO[0m\ie_to_edge_bho_64.dll ([0m[1;31mUnquoted and Space detected[0m) - C:\
[1;90m   =================================================================================================[0m


    RegPath: [0m[1;32mHKLM\Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Explorer\Browser Helper Objects\{1FD49718-1D00-4B19-AF5F-070AF6D5D54C}[0m
    Folder: [0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\128.0.2739.54\BHO[0m
    File: [0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application\128.0.2739.54\BHO[0m\ie_to_edge_bho_64.dll ([0m[1;31mUnquoted and Space detected[0m) - C:\
[1;90m   =================================================================================================[0m


    Folder: [0m[1;32mC:\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup[0m
    File: [0m[1;32mC:\ProgramData\Microsoft\Windows\Start Menu\Programs\Startup[0m\desktop.ini
    [0m[1;31mPotentially sensitive file content:[0m LocalizedResourceName=@%SystemRoot%\system32\shell32.dll,-21787
[1;90m   =================================================================================================[0m


    Folder: [0m[1;31mC:\Users\alex\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup[0m
    [0m[1;31mFolderPerms: alex [AllAccess][0m
    File: [0m[1;31m[0m[1;31mC:\Users\alex\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup[0m[0m\desktop.ini ([0m[1;31mUnquoted and Space detected[0m) - C:\Users\alex\AppData\Roaming\Microsoft\Windows,[0m[1;31m[0m[1;31mC:\Users\alex\AppData\Roaming\Microsoft\Windows\Start Menu\Programs\Startup[0m[0m\desktop.ini 
    [0m[1;31mFilePerms: alex [AllAccess][0m
    [0m[1;31mPotentially sensitive file content:[0m LocalizedResourceName=@%SystemRoot%\system32\shell32.dll,-21787
[1;90m   =================================================================================================[0m


    Folder: [0m[1;31mC:\windows\tasks[0m
    [0m[1;31mFolderPerms: Authenticated Users [WriteData/CreateFiles][0m
[1;90m   =================================================================================================[0m


    Folder: [0m[1;31mC:\windows\system32\tasks[0m
    [0m[1;31mFolderPerms: Authenticated Users [WriteData/CreateFiles][0m
[1;90m   =================================================================================================[0m


    Folder: [0m[1;32mC:\windows[0m
    File: [0m[1;32mC:\windows[0m\system.ini
[1;90m   =================================================================================================[0m


    Folder: [0m[1;32mC:\windows[0m
    File: [0m[1;32mC:\windows[0m\win.ini
[1;90m   =================================================================================================[0m


    Key: From WMIC
    Folder: [0m[1;31mC:\Users\alex\AppData\Local\Microsoft\OneDrive[0m
    [0m[1;31mFolderPerms: alex [AllAccess][0m
    File: [0m[1;31mC:\Users\alex\AppData\Local\Microsoft\OneDrive[0m\OneDrive.exe /background
    [0m[1;31mFilePerms: alex [AllAccess][0m
[1;90m   =================================================================================================[0m


    Key: From WMIC
    Folder: [0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application[0m
    File: [0m[1;32mC:\Program Files (x86)\Microsoft\Edge\Application[0m\msedge.exe --no-startup-window --win-session-start
[1;90m   =================================================================================================[0m


    Key: From WMIC
    Folder: [0m[1;32mC:\Windows\system32[0m
    File: [0m[1;32mC:\Windows\system32[0m\SecurityHealthSystray.exe
[1;90m   =================================================================================================[0m


    Key: From WMIC
    Folder: [0m[1;32mC:\Program Files\VMware\VMware Tools[0m
    File: [0m[1;32mC:\Program Files\VMware\VMware Tools[0m\vmtoolsd.exe -n vmusr
[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mScheduled Applications --Non Microsoft--[0m
[1;36m╚ [1;34mCheck if you can modify other users scheduled binaries [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation/privilege-escalation-with-autorun-binaries[0m

[1;36m╔══════════╣ [1;32mDevice Drivers --Non Microsoft--[0m
[1;36m╚ [1;34mCheck 3rd party drivers for known vulnerabilities/rootkits. [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#vulnerable-drivers[0m
    NVIDIA nForce(TM) RAID Driver - 10.6.0.23 [NVIDIA Corporation]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\nvraid.sys[0m
    QLogic 10 GigE - 7.13.65.105 [QLogic Corporation]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\evbd0a.sys[0m
    QLogic 10 GigE - 7.13.171.102 [Marvell Semiconductor Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\evbda.sys[0m
    QLogic Gigabit Ethernet - 7.12.31.105 [QLogic Corporation]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\bxvbda.sys[0m
    VMware vSockets Service - 9.8.19.0 build-18956547 [VMware, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\system32\DRIVERS\vsock.sys[0m
    VMware PCI VMCI Bus Device - 9.8.18.0 build-18956547 [VMware, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\vmci.sys[0m
    Intel Matrix Storage Manager driver - 8.6.2.1019 [Intel Corporation]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\iaStorV.sys[0m
    VIA RAID driver - 7.0.9600,6352 [VIA Technologies Inc.,Ltd]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\vsmraid.sys[0m
    Boot Camp - 6.1.0.0 [Apple Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\AppleSSD.sys[0m
    LSI 3ware RAID Controller - WindowsBlue [LSI]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\3ware.sys[0m
    AHCI 1.3 Device Driver - 1.1.3.277 [Advanced Micro Devices]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\amdsata.sys[0m
    Storage Filter Driver - 1.1.3.277 [Advanced Micro Devices]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\amdxata.sys[0m
    AMD Technology AHCI Compatible Controller - 3.7.1540.43 [AMD Technologies Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\amdsbs.sys[0m
    Adaptec RAID Controller - 7.5.0.32048 [PMC-Sierra, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\arcsas.sys[0m
    Windows (R) Win 7 DDK driver - 10.0.10011.16384 [Avago Technologies]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\ItSas35i.sys[0m
    LSI Fusion-MPT SAS Driver (StorPort) - 1.34.03.83 [LSI Corporation]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\lsi_sas.sys[0m
    Windows (R) Win 7 DDK driver - 10.0.10011.16384 [LSI Corporation]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\lsi_sas2i.sys[0m
    Windows (R) Win 7 DDK driver - 10.0.10011.16384 [Avago Technologies]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\lsi_sas3i.sys[0m
    MEGASAS2i RAID Controller Driver for Windows - 6.714.22.00 [Avago Technologies]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\MegaSas2i.sys[0m
    MEGASAS RAID Controller Driver for Windows - 7.717.02.00 [Broadcom Inc]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\megasas35i.sys[0m
    MegaRAID Software RAID - 15.02.2013.0129 [LSI Corporation, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\megasr.sys[0m
    Windows (R) Win 7 DDK driver - 10.0.10011.16384 [Broadcom Limited]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\mpi3drvi.sys[0m
    Marvell Flash Controller -  1.0.5.1016  [Marvell Semiconductor, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\mvumis.sys[0m
    NVIDIA nForce(TM) SATA Driver - 10.6.0.23 [NVIDIA Corporation]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\nvstor.sys[0m
    MEGASAS RAID Controller Driver for Windows - 6.805.03.00 [Avago Technologies]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\percsas2i.sys[0m
    MEGASAS RAID Controller Driver for Windows - 6.604.06.00 [Avago Technologies]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\percsas3i.sys[0m
    Microsoftr Windowsr Operating System - 2.60.01 [Silicon Integrated Systems Corp.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\SiSRaid2.sys[0m
    Microsoftr Windowsr Operating System - 6.1.6918.0 [Silicon Integrated Systems]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\sisraid4.sys[0m
    VIA StorX RAID Controller Driver - 8.0.9200.8110 [VIA Corporation]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\vstxraid.sys[0m
     Promiser SuperTrak EX Series -  5.1.0000.10 [Promise Technology, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\stexstor.sys[0m
    Chelsio Communications iSCSI Controller - 10.0.10011.16384 [Chelsio Communications]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\cht4sx64.sys[0m
    Intel(R) Rapid Storage Technology driver (inbox) - 15.44.0.1015 [Intel Corporation]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\iaStorAVC.sys[0m
    VMware PVSCSI StorPort driver (64-bit) - 1.3.25.0 build-19569981 [VMware, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\pvscsi.sys[0m
    PMC-Sierra HBA Controller - 1.3.0.10769 [PMC-Sierra]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\ADP80XX.SYS[0m
    Smart Array SAS/SATA Controller Media Driver - 8.0.4.0 Build 1 Media Driver (x86-64) [Hewlett-Packard Company]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\HpSAMD.sys[0m
    SmartRAID, SmartHBA PQI Storport Driver - 1.50.1.0 [Microsemi Corportation]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\SmartSAMD.sys[0m
    VMware Pointing USB Device Driver - 12.5.12.0 build-18933738 [VMware, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\vmusbmouse.sys[0m
    VMware Pointing PS/2 Device Driver - 12.5.12.0 build-18967789 [VMware, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\vmmouse.sys[0m
    VMware SVGA 3D - 9.17.01.0002 - build-18913173 [VMware, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\system32\DRIVERS\vm3dmp_loader.sys[0m
    VMware SVGA 3D - 9.17.01.0002 - build-18913173 [VMware, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\system32\DRIVERS\vm3dmp.sys[0m
    VMware server memory controller - 7.5.7.0 build-18933738 [VMware, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\system32\DRIVERS\vmmemctl.sys[0m
    VMware PCIe Ethernet Adapter NDIS 6.85 (64-bit) - 1.9.9.0 build-19932667 [VMware, Inc.]: [0m[1;32m\\.\GLOBALROOT\SystemRoot\System32\drivers\vmxnet3.sys[0m


[1;36m════════════════════════════════════╣ [1;32mNetwork Information[1;36m ╠════════════════════════════════════[0m

[1;36m╔══════════╣ [1;32mNetwork Shares[0m
    [0m[1;32mADMIN$[0m ([1;37mPath: C:\Windows[0m)
    [0m[1;32mC$[0m ([1;37mPath: C:\[0m)
    [0m[1;32mIPC$[0m ([1;37mPath: [0m)

[1;36m╔══════════╣ [1;32mEnumerate Network Mapped Drives (WMI)[0m

[1;36m╔══════════╣ [1;32mHost File[0m

[1;36m╔══════════╣ [1;32mNetwork Ifaces and known hosts[0m
[1;36m╚ [1;34mThe masks are only for the IPv4 addresses [1;33m[0m
    Ethernet0[00:50:56:BF:38:62]: 192.168.164.222, fe80::20fe:fbc1:d6e3:aa8f%6 / 255.255.255.0
        [1;37mGateways: [0m192.168.164.254
        [1;37mDNSs: [0m192.168.164.254
        [1;37mKnown hosts:[0m
          192.168.164.254       00-50-56-BF-4A-CD     Dynamic
          192.168.164.255       FF-FF-FF-FF-FF-FF     Static
          224.0.0.22            01-00-5E-00-00-16     Static
          224.0.0.251           01-00-5E-00-00-FB     Static
          224.0.0.252           01-00-5E-00-00-FC     Static
          239.255.255.250       01-00-5E-7F-FF-FA     Static

    Loopback Pseudo-Interface 1[]: 127.0.0.1, ::1 / 255.0.0.0
        [1;37mDNSs: [0mfec0:0:0:ffff::1%1, fec0:0:0:ffff::2%1, fec0:0:0:ffff::3%1
        [1;37mKnown hosts:[0m
          224.0.0.22            00-00-00-00-00-00     Static
          224.0.0.251           00-00-00-00-00-00     Static
          239.255.255.250       00-00-00-00-00-00     Static


[1;36m╔══════════╣ [1;32mCurrent TCP Listening Ports[0m
[1;36m╚ [1;34mCheck for services restricted from the outside [1;33m[0m
[1;34m  Enumerating IPv4 connections
[0m
  Protocol   Local Address         Local Port    Remote Address        Remote Port     State             Process ID      Process Name

  TCP        0.0.0.0               135           0.0.0.0               0               Listening         936             svchost
  TCP        0.0.0.0               445           0.0.0.0               0               Listening         4               System
  TCP        0.0.0.0               3389          0.0.0.0               0               Listening         704             svchost
  TCP        0.0.0.0               5040          0.0.0.0               0               Listening         5648            svchost
  TCP        0.0.0.0               5985          0.0.0.0               0               Listening         4               System
  TCP        0.0.0.0               7680          0.0.0.0               0               Listening         1148            svchost
  TCP        0.0.0.0               47001         0.0.0.0               0               Listening         4               System
  TCP        0.0.0.0               49664         0.0.0.0               0               Listening         708             lsass
  TCP        0.0.0.0               49665         0.0.0.0               0               Listening         568             wininit
  TCP        0.0.0.0               49666         0.0.0.0               0               Listening         1740            svchost
  TCP        0.0.0.0               49667         0.0.0.0               0               Listening         1960            svchost
  TCP        0.0.0.0               49668         0.0.0.0               0               Listening         2080            svchost
  TCP        0.0.0.0               49669         0.0.0.0               0               Listening         676             services
  TCP        0.0.0.0               49670         0.0.0.0               0               Listening         2872            svchost
  TCP        192.168.164.222       139           0.0.0.0               0               Listening         4               System
  TCP        192.168.164.222       3389          192.168.45.213        56164           Established       704             svchost
  TCP        192.168.164.222       4444          192.168.45.213        35250           Established       7040            nc
  TCP        192.168.164.222       54388         20.50.201.200         443             SYN Sent          7224            C:\Program Files\WindowsApps\MicrosoftTeams_24215.1105.3082.1600_x64__8wekyb3d8bbwe\msteams.exe
  TCP        192.168.164.222       54389         20.50.201.200         443             SYN Sent          7224            C:\Program Files\WindowsApps\MicrosoftTeams_24215.1105.3082.1600_x64__8wekyb3d8bbwe\msteams.exe
  TCP        192.168.164.222       54390         23.223.17.133         443             SYN Sent          8468            C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe
  TCP        192.168.164.222       54391         23.223.17.133         443             SYN Sent          8468            C:\Program Files (x86)\Microsoft\EdgeWebView\Application\128.0.2739.54\msedgewebview2.exe
  TCP        192.168.164.222       54392         172.172.255.216       443             SYN Sent          3064            svchost
  TCP        192.168.164.222       54393         52.113.194.132        443             SYN Sent          2860            MpDefenderCoreService
[0m[0m
[1;34m  Enumerating IPv6 connections
[0m
  Protocol   Local Address                               Local Port    Remote Address                              Remote Port     State             Process ID      Process Name

  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        135           [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         936             svchost
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        445           [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         4               System
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        3389          [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         704             svchost
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        5985          [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         4               System
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        7680          [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         1148            svchost
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        47001         [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         4               System
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        49664         [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         708             lsass
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        49665         [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         568             wininit
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        49666         [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         1740            svchost
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        49667         [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         1960            svchost
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        49668         [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         2080            svchost
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        49669         [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         676             services
  TCP        [0m[1;31m[0m[1;31m[::][0m[0m                                        49670         [0m[1;31m[0m[1;31m[::][0m[0m                                        0               Listening         2872            svchost

[1;36m╔══════════╣ [1;32mCurrent UDP Listening Ports[0m
[1;36m╚ [1;34mCheck for services restricted from the outside [1;33m[0m
[1;34m  Enumerating IPv4 connections
[0m
  Protocol   Local Address         Local Port    Remote Address:Remote Port     Process ID        Process Name

  UDP        0.0.0.0               123           *:*                            4600              svchost
  UDP        0.0.0.0               500           *:*                            2784              svchost
  UDP        0.0.0.0               3389          *:*                            704               svchost
  UDP        0.0.0.0               3702          *:*                            7484              svchost
  UDP        0.0.0.0               3702          *:*                            7484              svchost
  UDP        0.0.0.0               4500          *:*                            2784              svchost
  UDP        0.0.0.0               5050          *:*                            5648              svchost
  UDP        0.0.0.0               5353          *:*                            1564              svchost
  UDP        0.0.0.0               5355          *:*                            1564              svchost
  UDP        0.0.0.0               56575         *:*                            1564              svchost
  UDP        0.0.0.0               58817         *:*                            1564              svchost
  UDP        0.0.0.0               59143         *:*                            7484              svchost
  UDP        0.0.0.0               59289         *:*                            1564              svchost
  UDP        [0m[1;31m127.0.0.1[0m             1900          *:*                            5424              svchost
  UDP        [0m[1;31m127.0.0.1[0m             51032         *:*                            2808              svchost
  UDP        [0m[1;31m127.0.0.1[0m             62383         *:*                            5424              svchost
  UDP        192.168.164.222       137           *:*                            4                 System
  UDP        192.168.164.222       138           *:*                            4                 System
  UDP        192.168.164.222       1900          *:*                            5424              svchost
  UDP        192.168.164.222       62382         *:*                            5424              svchost
[0m[0m
[1;34m  Enumerating IPv6 connections
[0m
  Protocol   Local Address                               Local Port    Remote Address:Remote Port     Process ID        Process Name

  UDP        [0m[1;31m[::][0m                                        123           *:*                            4600              svchost
  UDP        [0m[1;31m[::][0m                                        500           *:*                            2784              svchost
  UDP        [0m[1;31m[::][0m                                        3389          *:*                            704               svchost
  UDP        [0m[1;31m[::][0m                                        3702          *:*                            7484              svchost
  UDP        [0m[1;31m[::][0m                                        3702          *:*                            7484              svchost
  UDP        [0m[1;31m[::][0m                                        4500          *:*                            2784              svchost
  UDP        [0m[1;31m[::][0m                                        5353          *:*                            1564              svchost
  UDP        [0m[1;31m[::][0m                                        5355          *:*                            1564              svchost
  UDP        [0m[1;31m[::][0m                                        56575         *:*                            1564              svchost
  UDP        [0m[1;31m[::][0m                                        58817         *:*                            1564              svchost
  UDP        [0m[1;31m[::][0m                                        59144         *:*                            7484              svchost
  UDP        [0m[1;31m[::][0m                                        59289         *:*                            1564              svchost
  UDP        [0m[1;31m[::1][0m                                       1900          *:*                            5424              svchost
  UDP        [0m[1;31m[::1][0m                                       62381         *:*                            5424              svchost
  UDP        [fe80::20fe:fbc1:d6e3:aa8f%6]               1900          *:*                            5424              svchost
  UDP        [fe80::20fe:fbc1:d6e3:aa8f%6]               62380         *:*                            5424              svchost

[1;36m╔══════════╣ [1;32mFirewall Rules[0m
[1;36m╚ [1;34mShowing only DENY rules (too many ALLOW rules always) [1;33m[0m
    Current Profiles: PUBLIC
    FirewallEnabled (Domain):    [0m[1;31mFalse[0m
    FirewallEnabled (Private):    [0m[1;31mFalse[0m
    FirewallEnabled (Public):    [0m[1;31mFalse[0m
[1;90m    DENY rules:[0m

[1;36m╔══════════╣ [1;32mDNS cached --limit 70--[0m
[1;90m    Entry                                 Name                                  Data[0m
    crl3.digicert.com                     crl3.digicert.com                     crl.edge.digicert.com
    crl3.digicert.com                     crl.edge.digicert.com                 fp2e7a.wpc.2be4.phicdn.net
    crl3.digicert.com                     fp2e7a.wpc.2be4.phicdn.net            fp2e7a.wpc.phicdn.net
    crl3.digicert.com                     fp2e7a.wpc.phicdn.net                 192.229.211.108
    ocsp.digicert.com                     ocsp.digicert.com                     ocsp.edge.digicert.com
    ocsp.digicert.com                     ocsp.edge.digicert.com                fp2e7a.wpc.2be4.phicdn.net
    ocsp.digicert.com                     fp2e7a.wpc.2be4.phicdn.net            fp2e7a.wpc.phicdn.net
    ocsp.digicert.com                     fp2e7a.wpc.phicdn.net                 192.229.211.108
    crl4.digicert.com                     crl4.digicert.com                     crl.edge.digicert.com
    crl4.digicert.com                     crl.edge.digicert.com                 fp2e7a.wpc.2be4.phicdn.net
    crl4.digicert.com                     fp2e7a.wpc.2be4.phicdn.net            fp2e7a.wpc.phicdn.net
    crl4.digicert.com                     fp2e7a.wpc.phicdn.net                 192.229.211.108
    ecs.office.com                        ecs.office.com                        ecs.office.trafficmanager.net
    ecs.office.com                        ecs.office.trafficmanager.net         s-0005-office.config.skype.com
    ecs.office.com                        s-0005-office.config.skype.com        ecs-office.s-0005.s-msedge.net
    ecs.office.com                        ecs-office.s-0005.s-msedge.net        s-0005.s-msedge.net
    ecs.office.com                        s-0005.s-msedge.net                   52.113.194.132
    client.wns.windows.com                client.wns.windows.com                wns.notify.trafficmanager.net
    client.wns.windows.com                wns.notify.trafficmanager.net         172.172.255.216
    client.wns.windows.com                client.wns.windows.com                wns.notify.trafficmanager.net
    client.wns.windows.com                wns.notify.trafficmanager.net         172.172.255.216

[1;36m╔══════════╣ [1;32mEnumerating Internet settings, zone and proxy configuration[0m
[1;34m  General Settings[0m
  Hive        Key                                       Value
  HKCU        CertificateRevocation                     1
  HKCU        DisableCachingOfSSLPages                  0
  HKCU        IE5_UA_Backup_Flag                        5.0
  HKCU        PrivacyAdvanced                           1
  HKCU        SecureProtocols                           10240
  HKCU        User Agent                                Mozilla/4.0 (compatible; MSIE 8.0; Win32)
  HKCU        ZonesSecurityUpgrade                      System.Byte[]
  HKCU        WarnonZoneCrossing                        0
  HKCU        EnableNegotiate                           1
  HKCU        ProxyEnable                               0
  HKCU        MigrateProxy                              1
  HKLM        ActiveXCache                              C:\Windows\Downloaded Program Files
  HKLM        CodeBaseSearchPath                        CODEBASE
  HKLM        EnablePunycode                            1
  HKLM        MinorVersion                              0
  HKLM        WarnOnIntranet                            1
[1;34m
  Zone Maps[0m
  No URLs configured
[1;34m
  Zone Auth Settings[0m
  No Zone Auth Settings


[1;36m════════════════════════════════════╣ [1;32mCloud Information[1;36m ╠════════════════════════════════════[0m
Learn and practice cloud hacking in [0m[1;32mtraining.hacktricks.xyz[0m
AWS EC2?                                No   
Azure VM?                               No   
Google Cloud Platform?                  No   
Google Workspace Joined?                No   
Google Cloud Directory Sync?            No   
Google Password Sync?                   No   


[1;36m════════════════════════════════════╣ [1;32mWindows Credentials[1;36m ╠════════════════════════════════════[0m

[1;36m╔══════════╣ [1;32mChecking Windows Vault[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#credentials-manager-windows-vault[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mChecking Credential manager[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#credentials-manager-windows-vault[0m
    [!] [0m[33mWarning:[0m if password contains non-printable characters, it will be printed as unicode base64 encoded string


  [!] Unable to enumerate credentials automatically, error: 'Win32Exception: System.ComponentModel.Win32Exception (0x80004005): Element not found'
Please run: 
[33mcmdkey /list[0m

[1;36m╔══════════╣ [1;32mSaved RDP connections[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mRemote Desktop Server/Client Settings[0m
[1;34m  RDP Server Settings[0m
    Network Level Authentication            :       
    Block Clipboard Redirection             :       
    Block COM Port Redirection              :       
    Block Drive Redirection                 :       
    Block LPT Port Redirection              :       
    Block PnP Device Redirection            :       
    Block Printer Redirection               :       
    Allow Smart Card Redirection            :       
[1;34m
  RDP Client Settings[0m
    Disable Password Saving                 :       True
    Restricted Remote Administration        :       False

[1;36m╔══════════╣ [1;32mRecently run commands[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mChecking for DPAPI Master Keys[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#dpapi[0m
[1;37m    MasterKey: [0mC:\Users\alex\AppData\Roaming\Microsoft\Protect\S-1-5-21-3557295818-2536705713-589665162-1003\27c5afc3-2aaf-4bb1-aeb9-feaed1a6745b
[1;37m    Accessed: [0m12/6/2024 8:11:04 AM
[1;37m    Modified: [0m9/16/2022 11:22:32 AM
[1;90m   =================================================================================================[0m

[1;37m    MasterKey: [0mC:\Users\alex\AppData\Roaming\Microsoft\Protect\S-1-5-21-3557295818-2536705713-589665162-1003\acb70894-02bb-452f-9f22-ad18ab769780
[1;37m    Accessed: [0m12/6/2024 8:11:04 AM
[1;37m    Modified: [0m12/6/2024 7:55:58 AM
[1;90m   =================================================================================================[0m

[1;37m    MasterKey: [0mC:\Users\alex\AppData\Roaming\Microsoft\Protect\S-1-5-21-3557295818-2536705713-589665162-1003\d5db6057-642a-48e0-9269-324cb9795fef
[1;37m    Accessed: [0m12/6/2024 8:03:31 AM
[1;37m    Modified: [0m9/3/2024 5:49:45 AM
[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mChecking for DPAPI Credential Files[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#dpapi[0m
[1;37m    CredFile: [0mC:\Users\alex\AppData\Local\Microsoft\Credentials\DFBE70A7E5CC19A398EBF1B96859CE5D
[1;37m    Description: [0mLocal Credential Data
  
[1;37m    MasterKey: [0macb70894-02bb-452f-9f22-ad18ab769780
[1;37m    Accessed: [0m12/6/2024 8:03:55 AM
[1;37m    Modified: [0m12/6/2024 8:01:06 AM
[1;37m    Size: [0m11152
[1;90m   =================================================================================================[0m

[1;36m╚ [1;34mFollow the provided link for further instructions in how to decrypt the creds file[0m

[1;36m╔══════════╣ [1;32mChecking for RDCMan Settings Files[0m
[1;36m╚ [1;34mDump credentials from Remote Desktop Connection Manager [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#remote-desktop-credential-manager[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mLooking for Kerberos tickets[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/pentesting/pentesting-kerberos-88[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mLooking for saved Wifi credentials[0m
[1;90m  [X] Exception: The service has not been started[0m
Enumerating WLAN using wlanapi.dll failed, trying to enumerate using 'netsh'
No saved Wifi credentials found

[1;36m╔══════════╣ [1;32mLooking AppCmd.exe[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#appcmd.exe[0m
[1;90m    Not Found[0m
      You must be an administrator to run this check

[1;36m╔══════════╣ [1;32mLooking SSClient.exe[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#scclient-sccm[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mEnumerating SSCM - System Center Configuration Manager settings[0m

[1;36m╔══════════╣ [1;32mEnumerating Security Packages Credentials[0m
[1;31m  Version: NetNTLMv2
  Hash:    alex::CLIENTWK222:1122334455667788:748cff18bb320f0acde6e891e79b264a:0101000000000000ab6d6123fa47db0126607b82e76f62df0000000008003000300000000000000000000000002000005410db445d9805528ffbaf53e6b6b35f407831b95e8b5b3e1b5568b8400bffa40a00100000000000000000000000000000000000090000000000000000000000
[0m
[1;90m   =================================================================================================[0m



[1;36m════════════════════════════════════╣ [1;32mBrowsers Information[1;36m ╠════════════════════════════════════[0m

[1;36m╔══════════╣ [1;32mShowing saved credentials for Firefox[0m
[33m    Info: if no credentials were listed, you might need to close the browser and try again.[0m

[1;36m╔══════════╣ [1;32mLooking for Firefox DBs[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#browsers-history[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mLooking for GET credentials in Firefox history[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#browsers-history[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mShowing saved credentials for Chrome[0m
[33m    Info: if no credentials were listed, you might need to close the browser and try again.[0m

[1;36m╔══════════╣ [1;32mLooking for Chrome DBs[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#browsers-history[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mLooking for GET credentials in Chrome history[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#browsers-history[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mChrome bookmarks[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mShowing saved credentials for Opera[0m
[33m    Info: if no credentials were listed, you might need to close the browser and try again.[0m

[1;36m╔══════════╣ [1;32mShowing saved credentials for Brave Browser[0m
[33m    Info: if no credentials were listed, you might need to close the browser and try again.[0m

[1;36m╔══════════╣ [1;32mShowing saved credentials for Internet Explorer (unsupported)[0m
[33m    Info: if no credentials were listed, you might need to close the browser and try again.[0m

[1;36m╔══════════╣ [1;32mCurrent IE tabs[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#browsers-history[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mLooking for GET credentials in IE history[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#browsers-history[0m


[1;36m╔══════════╣ [1;32mIE history -- limit 50
[0m
    http://go.microsoft.com/fwlink/p/?LinkId=255141

[1;36m╔══════════╣ [1;32mIE favorites[0m
    http://go.microsoft.com/fwlink/p/?LinkId=255142


[1;36m════════════════════════════════════╣ [1;32mInteresting files and registry[1;36m ╠════════════════════════════════════[0m

[1;36m╔══════════╣ [1;32mPutty Sessions[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mPutty SSH Host keys[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mSSH keys in registry[0m
[1;36m╚ [1;34mIf you find anything here, follow the link to learn how to decrypt the SSH keys [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#ssh-keys-in-registry[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mSuperPutty configuration files[0m

[1;36m╔══════════╣ [1;32mEnumerating Office 365 endpoints synced by OneDrive.
[0m
    SID: S-1-5-19
[1;90m   =================================================================================================[0m

    SID: S-1-5-20
[1;90m   =================================================================================================[0m

    SID: S-1-5-21-3557295818-2536705713-589665162-1002
[1;90m   =================================================================================================[0m

    SID: S-1-5-21-3557295818-2536705713-589665162-1003
[1;90m   =================================================================================================[0m

    SID: S-1-5-21-3557295818-2536705713-589665162-1004
[1;90m   =================================================================================================[0m

    SID: S-1-5-18
[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mCloud Credentials[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#credentials-inside-files[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mUnattend Files[0m

[1;36m╔══════════╣ [1;32mLooking for common SAM & SYSTEM backups[0m

[1;36m╔══════════╣ [1;32mLooking for McAfee Sitelist.xml Files[0m

[1;36m╔══════════╣ [1;32mCached GPP Passwords[0m

[1;36m╔══════════╣ [1;32mLooking for possible regs with creds[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#inside-the-registry[0m
[1;90m    Not Found[0m
[1;90m    Not Found[0m
[1;90m    Not Found[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mLooking for possible password files in users homes[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#credentials-inside-files[0m
    C:\Users\All Users\Microsoft\UEV\InboxTemplates\Roaming[0m[1;31mCredential[0mSettings.xml
    C:\Users\alex\AppData\Local\Packages\MicrosoftTeams_8wekyb3d8bbwe\LocalCache\Microsoft\MSTeams\EBWebView\ZxcvbnData\3.0.0.0\[0m[1;31mpassword[0ms.txt

[1;36m╔══════════╣ [1;32mSearching for Oracle SQL Developer config files
[0m

[1;36m╔══════════╣ [1;32mSlack files & directories[0m
[33m  note: check manually if something is found[0m

[1;36m╔══════════╣ [1;32mLooking for LOL Binaries and Scripts (can be slow)[0m
[1;36m╚ [1;34m [1;33mhttps://lolbas-project.github.io/[0m
[33m   [!] Check skipped, if you want to run it, please specify '-lolbas' argument[0m

[1;36m╔══════════╣ [1;32mEnumerating Outlook download files
[0m

[1;36m╔══════════╣ [1;32mEnumerating machine and user certificate files
[0m

[1;36m╔══════════╣ [1;32mSearching known files that can contain creds in home[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#credentials-inside-files[0m

[1;36m╔══════════╣ [1;32mLooking for documents --limit 100--[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mOffice Most Recent Files -- limit 50
[0m
[1;34m  Last Access Date           User                                           Application           Document[0m

[1;36m╔══════════╣ [1;32mRecent files --limit 70--[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mLooking inside the Recycle Bin for creds files[0m
[1;36m╚ [1;34m [1;33mhttps://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation#credentials-inside-files[0m
[1;90m    Not Found[0m

[1;36m╔══════════╣ [1;32mSearching hidden files or folders in C:\Users home (can be slow)
[0m
[1;31m     C:\Users\Default[0m
[1;31m     C:\Users\All Users[0m
[1;31m     C:\Users\All Users\ntuser.pol[0m
[1;31m     C:\Users\Default User[0m
[1;31m     C:\Users\Default[0m
[1;31m     C:\Users\All Users[0m
[1;31m     C:\Users\alex\AppData\Local\Temp\edge_BITS_412_1336911083\BITBDBD.tmp[0m

[1;36m╔══════════╣ [1;32mSearching interesting files in other users home directories (can be slow)
[0m
[1;32m     Checking folder: c:\users\administrator
[0m
[1;90m   =================================================================================================[0m

[1;32m     Checking folder: c:\users\diana
[0m
[1;90m   =================================================================================================[0m

[1;32m     Checking folder: c:\users\enterpriseadmin
[0m
[1;90m   =================================================================================================[0m

[1;32m     Checking folder: c:\users\enterpriseuser
[0m
[1;90m   =================================================================================================[0m

[1;32m     Checking folder: c:\users\offsec
[0m
[1;90m   =================================================================================================[0m


[1;36m╔══════════╣ [1;32mSearching executable files in non-default folders with write (equivalent) permissions (can be slow)[0m
     File Permissions "C:\Users\alex\Desktop\winPEASany.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\OneDrive\OneDriveStandaloneUpdater.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\OneDrive\OneDrive.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\wt.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\winget.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\SnippingTool.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\python3.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\python.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\pbrush.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\notepad.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\msteams_autostarter.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\msteamsupdate.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\msteams.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\mspaint.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\MicrosoftEdge.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\GameBarElevatedFT_Alias.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\MicrosoftTeams_8wekyb3d8bbwe\msteams_autostarter.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\MicrosoftTeams_8wekyb3d8bbwe\msteamsupdate.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\MicrosoftTeams_8wekyb3d8bbwe\msteams.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\Microsoft.XboxGamingOverlay_8wekyb3d8bbwe\GameBarElevatedFT_Alias.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\Microsoft.WindowsTerminal_8wekyb3d8bbwe\wt.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\Microsoft.WindowsNotepad_8wekyb3d8bbwe\notepad.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\Microsoft.ScreenSketch_8wekyb3d8bbwe\SnippingTool.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\Microsoft.Paint_8wekyb3d8bbwe\pbrush.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\Microsoft.Paint_8wekyb3d8bbwe\mspaint.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\Microsoft.MicrosoftEdge_8wekyb3d8bbwe\MicrosoftEdge.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\Microsoft.DesktopAppInstaller_8wekyb3d8bbwe\winget.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\Microsoft.DesktopAppInstaller_8wekyb3d8bbwe\python3.exe": alex [AllAccess]
     File Permissions "C:\Users\alex\AppData\Local\Microsoft\WindowsApps\Microsoft.DesktopAppInstaller_8wekyb3d8bbwe\python.exe": alex [AllAccess]
[1;31m     File Permissions "C:\Services\nc.exe": Authenticated Users [WriteData/CreateFiles][0m

[1;36m╔══════════╣ [1;32mLooking for Linux shells/distributions - wsl.exe, bash.exe[0m
[1;31m    C:\Windows\System32\wsl.exe[0m
[1;31m[0m
[1;32m    WSL - no installed Linux distributions found.[0m
[1;32m
       /---------------------------------------------------------------------------------\
       |                             [34mDo you like PEASS?[1;32m                                  |
       |---------------------------------------------------------------------------------| 
       |         [33mLearn Cloud Hacking[1;32m       :     [1;31mtraining.hacktricks.xyz[1;32m                 |
       |         [33mFollow on Twitter[1;32m         :     [1;31m@hacktricks_live[1;32m                        |
       |         [33mRespect on HTB[1;32m            :     [1;31mSirBroccoli            [1;32m                 |
       |---------------------------------------------------------------------------------|
       |                                 [34mThank you![1;32m                                      |
       \---------------------------------------------------------------------------------/
[0m

```