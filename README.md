## 1. Logs and Sigma Alerts
**Artifact name:** Windows.EventLogs.Evtx  
**Description:** All Windows Logs

**Artifact name:** Windows.EventLogs.Hayabusa  
**Description:** Sigma Alerts

## 2. Persistence

**Artifact name:** Windows.Sysinternals.Autoruns  
**Description:** Detects persistence mechanisms used by attackers (registry, scheduled tasks, services, etc.).

## 3. Installed Applications and Execution Traces

**Artifact name:** Windows.Sys.Programs  
**Description:** Identifies applications installed via Windows Installer.

**Artifact name:** Windows.Registry.UserAssist  
**Description:**  Programs executed via the graphical interface

**Artifact name:** Windows.Detection.Amcache  
**Description:** Files executed on the system; executable file hashes (SHA-1) can be retrieved  

**Artifact name:** Windows.Forensics.Prefetch  
**Description:** Program execution optimization; loaded DLLs can be identified  

**Artifact name:** Windows.Forensics.RecentApps  
**Description:**  Recently used applications

**Artifact name:** Windows.Forensics.Bam  
**Description:** BAM (Background Activity Moderator) is a Windows component that tracks background application activity.

**Artifact name:** Windows.Forensics.SRUM  
**Description:** SRUM (System Resource Usage Monitor) records application activity and network usage.

## 4. Network 

**Artifact name:** Windows.Sys.Interfaces  
**Description:** Lists Interfaces.

**Artifact name:** Windows.Registry.RDP  
**Description:** Lists all RDP connections recorded in the registry history.

**Artifact name:** Windows.System.Shares  
**Description:** Lists all system shares.

**Artifact name:** Windows.Registry.MountPoints2 (No regex)  
**Description:** Lists all Mount Points.

**Artifact name:** Windows.Sys.FirewallRules  
**Description:** Lists all Firewall Rules.

**Artifact name:** Windows.System.VBScript (run quser)  
**Description:** Used to display user sessions open on a Windows machine.
```
Set sh = CreateObject("WScript.Shell")
Set ex = sh.Exec("cmd /c quser")
WScript.Echo ex.StdOut.ReadAll()
```

## 5. User Accounts

**Artifact name:** Windows.Forensics.SAM  
**Description:** Lists all local user and administrator accounts.


## 6. Files and Activity Traces

**Artifact name:** Windows.Sys.DiskInfo  
**Description:** System disk info.

**Artifact name:** Windows.NTFS.MFT  
**Description:** Retrieves the Master File Table (MFT) to analyze file creation, modification, and access timestamps.

**Artifact name:** Windows.Forensics.Usn  
**Description:** Logs file modifications.

**Artifact name:** Windows.Forensics.Lnk  
**Description:** Recently visited files.

**Artifact name:** Windows.Forensics.Shellbags  
**Description:** Allows identification of accessed folder paths and names, even if they have been deleted.

**Artifact name:** Windows.Forensics.RDPCache  
**Description:** RDP Bitmap Cache.

**Artifact name:** Windows.NTFS.I30  
**Description:** Analyzes $I30 indexes to detect deleted files.

**Artifact name:** Windows.Analysis.EvidenceOfDownload  
**Description:** Identifies downloaded files through the presence of the Zone.Identifier stream.

**Artifact name:** Windows.Forensics.RecycleBin  
**Description:** Identifies files deleted to the Windows Recycle Bin ($Recycle.Bin).

**Artifact name:** Windows.Timeline.Registry.RunMRU  
**Description:** Command history from Windows + R.

**Artifact name:** Windows.Applications.Chrome.History  
**Description:** Chrome browsing history.

**Artifact name:** Windows.Applications.Edge.History  
**Description:** Edge browsing history.

**Artifact name:** Windows.Applications.Firefox.History  
**Description:** Firefox browsing history.


## 7. PowerShell Activity

**Artifact name:** Windows.System.Powershell.PSReadline  
**Description:** Collects the PowerShell command history.
