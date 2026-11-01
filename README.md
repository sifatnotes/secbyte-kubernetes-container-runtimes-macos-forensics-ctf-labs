# secbyte-kubernetes-container-runtimes-macos-forensics-ctf-labs
A practical collection of cybersecurity CTF labs covering Kubernetes admission controllers (OPA/Gatekeeper), OCI image specifications, container runtime escapes (runc), Kubernetes supply chain threats, and macOS forensics (Gatekeeper, XProtect, Launchd persistence, Keychain security, Endpoint Security framework).
# Kubernetes Policy Enforcement, Container Runtime Escapes & macOS Forensics CTF Labs

Welcome to the **Kubernetes Policy Enforcement, Container Runtime Escapes & macOS Forensics CTF Lab Collection**. This repository serves as an organized, searchable catalog of practical cybersecurity labs hosted on Learn SecByte.

This collection covers advanced cloud-native cluster governance, low-level container runtime breakout mechanics, and deep macOS forensic analysis—spanning **Kubernetes Policy Enforcement & Admission Controllers (OPA/Gatekeeper, Pod Security Admission)**, **Container Runtime Escapes & OCI Image Forensics (runc exploits, layer inspection, supply chain crosshairs)**, and **macOS Forensics, Malware Analysis & Security Subsystems (Gatekeeper, XProtect, Launchd persistence, Keychain secrets, Apple Endpoint Security)**.

---

## Lab Collection Index

### 1. Kubernetes Admission Controllers & Policy Governance
* **Kubernetes Admission Controllers: Policy Gatekeeper**  
  *Lab Link:* [https://learn.secbyte.org/ctf/kubernetes-admission-controllers-policy-gatekeeper](https://learn.secbyte.org/ctf/kubernetes-admission-controllers-policy-gatekeeper)  
  *Focus:* Implementing Open Policy Agent (OPA) / Gatekeeper constraints, writing custom Rego policy rules, enforcing Validating/Mutating Admission Webhooks, and blocking non-compliant pod deployments.

<Image src="image_agent_tag_12785009429713829614" alt="Kubernetes system component icons detailing deployments, scaling, and pod container management" caption="Kubernetes Control Plane & Policy Management Framework" />

---

### 2. Container Runtime Escapes & Image Layer Forensics
* **OCI Image Spec: Layer Cake Incident**  
  *Lab Link:* [https://learn.secbyte.org/ctf/oci-image-spec-layer-cake-incident](https://learn.secbyte.org/ctf/oci-image-spec-layer-cake-incident)  
  *Focus:* Dissecting OCI image manifest specifications, inspecting hidden layer diffs (`docker history`, `dive`), extracting embedded secrets across deleted image layers, and auditing base image provenance.

* **Container Runtime Security: runc Escape Audit**  
  *Lab Link:* [https://learn.secbyte.org/ctf/container-runtime-security-runc-escape-audit](https://learn.secbyte.org/ctf/container-runtime-security-runc-escape-audit)  
  *Focus:* Analyzing low-level container runtime breakouts (CVE-2019-5736 runc file descriptor overwrites), auditing file descriptor leaks, and hardening container runtime abstractions.

* **Containers in the Crosshairs: Kubernetes Escape and Supply Chain**  
  *Lab Link:* [https://learn.secbyte.org/ctf/containers-in-the-crosshairs-kubernetes-escape-and-supply-ch](https://learn.secbyte.org/ctf/containers-in-the-crosshairs-kubernetes-escape-and-supply-ch)  
  *Focus:* Executing end-to-end attack chains—from poisoning container registry dependencies to escaping Kubernetes pod boundaries onto host worker nodes.

### 3. macOS Subsystems, Security Controls & Telemetry
* **Gatekeeper Security: The Trailing Token**  
  *Lab Link:* [https://learn.secbyte.org/ctf/gatekeeper-security-the-trailing-token](https://learn.secbyte.org/ctf/gatekeeper-security-the-trailing-token)  
  *Focus:* Auditing macOS Gatekeeper validation checks, analyzing quarantine extended attributes (`com.apple.quarantine`), and testing bypass vectors involving code signing trailing data tokens.

<Image src="image_agent_tag_12785009429713828233" alt="macOS Gatekeeper and XProtect verification framework workflow diagram" caption="macOS Gatekeeper & XProtect Verification Flow" />

---

* **XProtect Analysis: The Orchard Breach**  
  *Lab Link:* [https://learn.secbyte.org/ctf/xprotect-analysis-the-orchard-breach](https://learn.secbyte.org/ctf/xprotect-analysis-the-orchard-breach)  
  *Focus:* Inspecting macOS XProtect YARA-based signature rules, analyzing XProtect Remediator execution behavior, and identifying malware signature evasion techniques.

* **Apple Endpoint Security: Broken Telemetry**  
  *Lab Link:* [https://learn.secbyte.org/ctf/apple-endpoint-security-broken-telemetry](https://learn.secbyte.org/ctf/apple-endpoint-security-broken-telemetry)  
  *Focus:* Auditing the Apple Endpoint Security (ES) API framework, detecting ES client suppression/tampering, and restoring system event telemetry feeds.

### 4. macOS Malware Analysis, Forensics & Persistence
* **Silent Orchard: macOS Malware Analysis**  
  *Lab Link:* [https://learn.secbyte.org/ctf/silent-orchard-macos-malware-analysis](https://learn.secbyte.org/ctf/silent-orchard-macos-malware-analysis)  
  *Focus:* Reverse-engineering Mach-O binaries, decompiling Objective-C/Swift samples, identifying dynamic library (`dylib`) hijacking, and analyzing C2 communication channels.

* **macOS Forensics: The Hidden Timeline**  
  *Lab Link:* [https://learn.secbyte.org/ctf/macos-forensics-the-hidden-timeline](https://learn.secbyte.org/ctf/macos-forensics-the-hidden-timeline)  
  *Focus:* Parsing Unified Logs (`log show`), analyzing macOS file system artifacts (APFS snapshots, fsevents, KnowledgeC.db), and constructing precise forensic incident timelines.

* **macOS Root Cause**  
  *Lab Link:* [https://learn.secbyte.org/ctf/macos-root-cause](https://learn.secbyte.org/ctf/macos-root-cause)  
  *Focus:* Executing root cause analysis on compromised macOS endpoints, determining initial execution vectors, and tracking privilege escalation mechanisms.

* **Launchd Shadows: Agents and Daemons**  
  *Lab Link:* [https://learn.secbyte.org/ctf/launchd-shadows-agents-and-daemons](https://learn.secbyte.org/ctf/launchd-shadows-agents-and-daemons)  
  *Focus:* Auditing user LaunchAgents and system LaunchDaemons (`plist` files in `/Library/LaunchDaemons` and `~/Library/LaunchAgents`), detecting persistence mechanisms, and cleaning rogue plist entries.

* **Keychain: Locks and Secrets**  
  *Lab Link:* [https://learn.secbyte.org/ctf/keychain-locks-and-secrets](https://learn.secbyte.org/ctf/keychain-locks-and-secrets)  
  *Focus:* Auditing macOS Keychain access controls, analyzing security item ACLs, extracting stored secrets, and investigating unauthorized access attempts via `security` CLI tools.

---

## Learning Path

### Path A: Kubernetes Policy & Container Runtime Specialist
1. **Cluster Governance:** Start with [Kubernetes Admission Controllers: Policy Gatekeeper](https://learn.secbyte.org/ctf/kubernetes-admission-controllers-policy-gatekeeper).
2. **Container Escapes & Image Audits:** Master runtime security via [OCI Image Spec: Layer Cake Incident](https://learn.secbyte.org/ctf/oci-image-spec-layer-cake-incident), [Container Runtime Security: runc Escape Audit](https://learn.secbyte.org/ctf/container-runtime-security-runc-escape-audit), and [Containers in the Crosshairs](https://learn.secbyte.org/ctf/containers-in-the-crosshairs-kubernetes-escape-and-supply-ch).

### Path B: macOS Security Subsystems & Defense Specialist
1. **Security Subsystems & Telemetry:** Audit core OS security controls in [Gatekeeper Security: The Trailing Token](https://learn.secbyte.org/ctf/gatekeeper-security-the-trailing-token), [XProtect Analysis](https://learn.secbyte.org/ctf/xprotect-analysis-the-orchard-breach), and [Apple Endpoint Security: Broken Telemetry](https://learn.secbyte.org/ctf/apple-endpoint-security-broken-telemetry).

### Path C: macOS Forensic Investigator & Malware Analyst
1. **Malware Analysis & Forensics:** Analyze Mach-O binaries in [Silent Orchard: macOS Malware Analysis](https://learn.secbyte.org/ctf/silent-orchard-macos-malware-analysis) and construct timelines in [macOS Forensics: The Hidden Timeline](https://learn.secbyte.org/ctf/macos-forensics-the-hidden-timeline) and [macOS Root Cause](https://learn.secbyte.org/ctf/macos-root-cause).
2. **Persistence & Secrets:** Audit host artifacts using [Launchd Shadows: Agents and Daemons](https://learn.secbyte.org/ctf/launchd-shadows-agents-and-daemons) and [Keychain: Locks and Secrets](https://learn.secbyte.org/ctf/keychain-locks-and-secrets).

---

## How to Use the Labs

1. Select a practice scenario from the **Lab Collection Index**.
2. Click the corresponding direct link to launch the exercise environment hosted on Learn SecByte.
3. Review scenario directives, OPA Rego policies, container layer files, Mach-O binaries, or macOS Unified Log exports.
4. Enforce OPA Gatekeeper constraints, exploit runc file descriptor leaks, decompile macOS malware, analyze LaunchDaemon plist persistence, or parse APFS file system timelines to capture flags.

---

## Target Audience

* **Cloud-Native & Kubernetes Security Engineers:** Configure OPA/Gatekeeper admission controllers, audit container runtime abstractions, and analyze container image layer secrets.
* **macOS Forensic Investigators & Incident Responders:** Parse macOS Unified Logs, analyze APFS artifacts, triage Launchd persistence, and investigate endpoint compromises.
* **Mac Malware Analysts & Reverse Engineers:** Reverse-engineer Mach-O binaries, analyze XProtect signatures, evaluate Gatekeeper bypass mechanisms, and inspect Keychain security.
* **Cybersecurity Students:** Acquire practical skills in cloud-native security, container runtime internals, and macOS forensics.

---

## Disclaimer

All lab links provided in this repository direct to official training environments hosted on Learn SecByte. All materials and exercises are provided strictly for educational purposes, defensive skill building, and authorized security research. Unauthorized scanning, probing, or exploiting of external container environments or macOS systems is strictly prohibited.
