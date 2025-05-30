
# 🔍 Phase 2 Investigation Report

## Hint 2: Malicious PowerShell Execution

**Objective:** Detect encoded or suspicious PowerShell commands, especially those launched by Office applications.

**Detection Strategies:**
- Monitor for parent-child process relationships such as `winword.exe → powershell.exe`.
- Look for encoded command strings typically using `-EncodedCommand`.
- Enable and analyze:
  - **Sysmon Event ID 1** – Process creation.
  - **Event ID 4104** – PowerShell script block logging (must be enabled via Group Policy).

**Tools:**
- Sysmon with enhanced PowerShell logging.
- Log parsers and SIEM tools.
