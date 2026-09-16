**TryHackMe Lab: Introductory Researching**
Category: Vulnerability Intelligence, Documentation Parsing, & Network Sockets

## Practical Methodology & Search Verification

1. **Vulnerability Data Retrieval (OSINT):**
   * Process: Analyzed legacy systems flaws and mapped global parameters utilizing open vulnerability databases (NVD / MITRE).
   * Key Findings: Tracked critical vulnerability vectors including WPForms XSS (CVE-2020-10385), Apache Tomcat Privilege Escalation (CVE-2016-1240), VLC initial root flaw (CVE-2007-0017), and Sudo Buffer Overflow (CVE-2019-18634).

2. **System Manual Extraction ('man' pages):**
   * Executed text queries within local manual boundaries to isolate operational flags.
   * Discovered `-r` switch for recursive directory transfers in `scp` and verified partitioning flags for `fdisk`.

3. **Network Listener Configuration (`nc`):**
   * Command Executed: `nc -l -p 12345`
   * Logic: Initialized a raw socket listener bound to local port 12345 using the listening (`-l`) and port selection (`-p`) parameters.

##  Core Academic Takeaway (Data Privacy Alignment)
Before engineering or deploying any privacy-preserving system architecture (like those researched at EPFL's SPRING Lab), an engineer must possess deep documentation literacy. Knowing how to query system manuals internally and map dependencies against global CVE data indices ensures that underlying infrastructure layers are secure against unauthorized metadata extraction vectors.
