
## Hint 8: Lateral Movement Simulation

**Objective:** Observe file access and transfer between systems to simulate attacker movement.

**Execution:**
- Copy an executable to a shared folder on another machine or VM.

**Detection Focus:**
- **SMB Access Logs** – Identify share access and file copy events.
- Analyze for Event IDs like:
  - **5140** – A network share was accessed.
  - **4663** – An object was accessed.

**Security Controls:**
- Use of firewalls, SMB restrictions, and endpoint monitoring to block or alert on suspicious file movements.

---
