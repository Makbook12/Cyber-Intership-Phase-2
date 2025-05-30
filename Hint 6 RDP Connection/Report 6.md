
## Hint 6: Unauthorized Remote Desktop Access

**Objective:** Detect RDP access attempts, both successful and failed.

**Detection Strategies:**
- Attempt login from a different IP.
- Key Event IDs to monitor:
  - **Event ID 4624** – Successful logon.
  - **Logon Type 10** – Remote interactive logon (RDP).

**Focus:**
- Source IP addresses, session types, and account used.
