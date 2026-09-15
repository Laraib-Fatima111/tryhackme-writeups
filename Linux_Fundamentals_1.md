#  TryHackMe Lab: Linux Fundamentals (Part 1)
**Category:** Operating System Infrastructure & Data Stream Redirection

##  Command Execution & Verification Evidence

1. **Directory Path Clarification:**
   * Command: `cd /home/tryhackme && ls`
   * Outcome: Successfully re-routed the structural terminal path to isolate the target user folders (`folder1`).

2. **File Data Extraction:**
   * Command: `cat folder1/password.txt`
   * Outcome: Successfully read the isolated password configuration file data string.

3. **Data Stream Overwriting vs. Appending (`>` vs `>>`):**
   * Command: `echo "TryHackMe" > thm`
   * Outcome: Initialized file `thm` and truncated any existing buffer to overwrite the file string.
   * Command: `echo "thm" >> thm`
   * Outcome: Safely appended the new string block to the EOF (End-of-File) marker without destroying existing structural data.
   * Verification: `cat thm` output confirmed the dual-line log structure.

##  Core Security & Privacy Takeaways
* **Forensic Integrity:** In production systems and security architecture logs, using the single `>` redirection character is a vulnerability because it erases historical logs. The double `>>` append operator is required to preserve data timelines for incident response analysis.
