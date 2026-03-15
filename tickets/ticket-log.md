## Ticket #001 — Process Monitoring
**Date:** 2026-03-14
**Tool used:** RustDesk (remote session to end-user PC)
**Steps taken:**
- Opened Task Manager via Ctrl+Shift+Esc
- Reviewed running processes — 70 background processes active
- Antimalware Service Executable noted at 202.8 MB memory usage, within acceptable range
- No hung or high CPU processes found

**Resolution:** No action required. System running normally.  
**Screenshot:** screenshots/taskmanager.png

---

## Ticket #002 — Driver Health Check
**Date:** 2026-03-14
**Tool used:** RustDesk (remote session to end-user PC)
**Steps taken:**
- Opened Device Manager
- Expanded Display Adapters — NVIDIA GeForce GTX 1660 Ti driver healthy
- Expanded Network Adapters — all adapters functioning normally
- Found one Unknown Device under Other Devices — flagged for follow-up

**Resolution:** All critical drivers healthy. Unknown device logged for further investigation.  
**Screenshot:** screenshots/devicemanager.png

---

## Ticket #003 — System Error Log Review
**Date:** 2026-03-14
**Tool used:** RustDesk (remote session to end-user PC)
**Steps taken:**
- Opened Event Viewer → Windows Logs
- Reviewed Summary of Administrative Events
- Found 70 errors over 7 days across multiple sources including Kernel, VSS, and DHCP
- No critical events found

**Resolution:** Error volume within normal range. No immediate action required.  
**Screenshot:** screenshots/eventviewer.png

---

## Ticket #004 — Temp File Cleanup
**Date:** 2026-03-14
**Tool used:** RustDesk (remote session to end-user PC)
**Steps taken:**
- Opened Run dialog → typed %temp%
- Selected all files and deleted
- Skipped shared_memory-rs folder as it was in use by a running process

**Resolution:** Temp files cleared successfully. One folder skipped due to active system use.  
**Screenshot:** screenshots/tempfiles.png

---

## Ticket #005 — System Specs Review
**Date:** 2026-03-14
**Tool used:** RustDesk (remote session to end-user PC)
**Steps taken:**
- Opened System Information
- Confirmed OS: Windows 10 Home, Build 19045
- Processor: Intel Core i5-9400 @ 2.90GHz
- System: Dell G5 5090, x64-based PC

**Resolution:** Specs documented. No issues found.  
**Screenshot:** screenshots/systeminfo.png