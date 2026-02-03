## 1. Persistence

**Artifact name:** Windows.Sysinternals.Autoruns  
**Description:** Detects persistence mechanisms used by attackers (registry, scheduled tasks, services, etc.).


## 2. Installed Applications and Execution Traces

**Artifact name:** Windows.Sys.Programs  
**Description:** Identifies applications installed via Windows Installer.

**Artifact name:** Windows.Analysis.EvidenceOfExecution  
**Description:** Centralizes all evidence of program execution across multiple sources.

- **UserAssist:** Programs executed via the graphical interface  
- **Amcache:** Files executed on the system; executable file hashes (SHA-1) can be retrieved  
- **Prefetch:** Program execution optimization; loaded DLLs can be identified  
- **RecentApps:** Recently used applications

**Artifact name:** Windows.Forensics.SRUM  
**Description:** SRUM (System Resource Usage Monitor) records application activity and network usage.

**Artifact name:** Generic.System.Pstree  
**Description:** Reconstructs the process tree to analyze relationships between executables.

**Artifact name:** Windows.System.DLLs  
**Description:** Enumerates DLLs loaded by a running process.

**Artifact name:** Windows.Sys.Drivers  
**Description:** Provides details on Windows drivers in use.


## 3. Network Activity

**Artifact name:** Windows.Registry.RDP  
**Description:** Lists all RDP connections recorded in the registry history.

**Artifact name:** Windows.Network.NetstatEnriched  
**Description:** Identifies processes initiating network connections.


## 4. User Accounts

**Artifact name:** Windows.Forensics.SAM  
**Description:** Lists all local user and administrator accounts.


## 5. Files and Activity Traces

**Artifact name:** Windows.NTFS.MFT  
**Description:** Retrieves the Master File Table (MFT) to analyze file creation, modification, and access timestamps.

**Artifact name:** Windows.Forensics.Usn  
**Description:** Logs file modifications.

**Artifact name:** Windows.Forensics.Lnk
**Description:** Recently visited files.

**Artifact name:** Windows.Forensics.Shellbags  
**Description:** Allows identification of accessed folder paths and names, even if they have been deleted.

**Artifact name:** Windows.NTFS.I30  
**Description:** Analyzes $I30 indexes to detect deleted files.

**Artifact name:** Windows.Analysis.EvidenceOfDownload  
**Description:** Identifies downloaded files through the presence of the Zone.Identifier stream.

**Artifact name:** Windows.Forensics.RecycleBin  
**Description:** Identifies files deleted to the Windows Recycle Bin ($Recycle.Bin).

**Artifact name:** Windows.Timeline.Registry.RunMRU 
**Description:** Command history from Windows+R.

**Artifact name:** Windows.Applications.Chrome.History 
**Description:** Chrome browsing history.

**Artifact name:** Windows.Applications.Edge.History  
**Description:** Edge browsing history.

**Artifact name:** Windows.Applications.Firefox.History  
**Description:** Firefox browsing history.


## 6. PowerShell Activity

**Artifact name:** Windows.EventLogs.PowershellScriptblock  
**Description:** Collects executed PowerShell scripts.

**Artifact name:** Windows.System.Powershell.PSReadline  
**Description:** Collects the PowerShell command history.
