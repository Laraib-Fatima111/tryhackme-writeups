#  TryHackMe Lab: Introductory Networking
**Category:** Network Diagnostics, Infrastructure Topology, & OSINT Registry Enumeration

##  Practical Methodology & Diagnostic Verification

1. **Domain Registry Intelligence Retrieval (WHOIS):**
   * Process: Executed deep architectural lookups targeting corporate infrastructure profiles (`facebook.com` and `microsoft.com`) to extract historical and geographical registration data.
   * Key Findings: Isolated legacy domain initialization vectors dating back to 1997, verified primary physical layout landmarks using geospatial OSINT markers (Bellevue infrastructure), and extracted authoritative points of contact (`msnhst@microsoft.com`).

2. **Domain Name System (DNS) Hierarchical Mapping:**
   * Analyzed logical namespace routing sequences. Documented that client operating systems prioritize the **Recursive DNS Server** as the primary external query terminal to traverse the root, TLD, and authoritative boundaries.
   * Documented core Anycast high-availability layouts including Google's secondary public resolver (`8.8.4.4`).
   * Validated temporal caching mechanics: Confirmed that a 24-hour Time-To-Live (TTL) constraint translates explicitly to a raw numeric counter of **86400 seconds** within terminal diagnostic tools like `dig`.

3. **ICMP Network Diagnostics (`ping`):**
   * Mechanism: Evaluated active packet transmission controls. Verified that the **`-i`** switch alters the temporal frequency (interval) of ICMP Echo Requests. Controlling this parameter is essential for fine-tuning diagnostic metrics and managing stateful firewall alert thresholds.

##  Core Academic Takeaway (Systems Architecture Alignment)
Deep networking literacy is a mandatory prerequisite for constructing distributed computational systems. Whether evaluating peer-to-peer applications or building privacy-preserving contact networks (such as those analyzed in elite research frameworks like EPFL), a systems engineer must thoroughly understand lower-level frame handling, TTL caching behavior, and network socket telemetry to prevent cross-border data leakage and transport-layer traffic profiling.
