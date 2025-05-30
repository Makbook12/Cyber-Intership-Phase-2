## Hint 10: Web Shell or Reverse Shell Execution

**Objective:** Detect the use of reverse shells and web shells for remote command execution.

**Execution:**
- Launch a reverse shell using **Netcat** or **PowerShell**.

**Detection Techniques:**
- Analyze abnormal parent-child process chains (e.g., `powershell.exe → nc.exe`).
- Look for:
  - Outbound traffic on unusual ports (e.g., 4444, 8081).
  - Processes without associated user sessions.

**Key Logs:**
- Sysmon Event IDs for network and process creation.
- Firewall logs for outbound connections.

