**Objective:** Identify periodic outbound connections indicative of Command & Control (C2) behavior.

**Detection Strategies:**
- Simulate scheduled HTTP/HTTPS pings to an external or custom domain.
- Analyze periodic outbound traffic patterns.

**Detection Tools:**
- **Wireshark / Zeek** – For packet analysis and flow inspection.
- **Firewall / Winlogbeat logs** – To track outgoing connections, domain resolution, and connection timings.

---
