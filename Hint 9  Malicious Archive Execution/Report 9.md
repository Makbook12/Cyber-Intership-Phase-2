## Hint 9: Malicious Archive Execution

**Objective:** Detect execution of malware delivered via password-protected archives.

**Execution:**
- Run an executable extracted from a protected ZIP/RAR archive.

**Detection Techniques:**
- Sysmon and AV logs:
  - **Event ID 1** – Process creation.
  - Track file hashes and original archive paths.
- Monitor for unexpected processes spawned by `explorer.exe` or decompression tools.
