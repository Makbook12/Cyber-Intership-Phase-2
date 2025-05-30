## Hint 5: Privilege Escalation Simulation

**Objective:** Track local privilege escalation attempts via user group modifications.

**Detection Strategies:**
- Add a local user to the Administrators group and monitor logs.
- Check for:
  - **Event ID 4728** – Member added to a global group.
  - **Event ID 4732** – Member added to a local security group.

**Analysis Approach:**
- Compare group membership snapshots before and after the operation.

