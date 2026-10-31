# Package Sentinel: Security & Governance for Azure Artifacts

[![Publisher](https://img.shields.io/badge/Publisher-Radwan%20Almsora-blue)](https://marketplace.visualstudio.com)
[![Version](https://img.shields.io/badge/Version-1.0.0-green)](#)
[![License](https://img.shields.io/badge/License-MIT-brightgreen)](#)

> **Package Sentinel** provides a consolidated view, governance, and security auditing for all your Azure Artifacts feeds in one place. It reads your real settings, compares them against configurable rules, and helps you remediate risks and perform safe cleanups. Package Sentinel operates entirely client-side, using no external servers and transmitting zero data.

---

## 📋 Table of Contents
- [Key Features](#-key-features)
- [Supported Feed Types](#-supported-feed-types)
- [Permissions & Privacy](#-permissions--privacy)
- [Quick Start](#-quick-start)
- [Detailed Features](#-detailed-features)
  - [1. Feed Security Audit](#1-feed-security-audit)
  - [2. Package Lifecycle Dashboard](#2-package-lifecycle-dashboard)
  - [3. Retention Policy Analyzer](#3-retention-policy-analyzer)
  - [4. Safe Cleanup Preview](#4-safe-cleanup-preview)
- [Support & Community](#-support--community)

---

## ✨ Key Features

* **Deterministic Security Audits:** Uncover broad permissions and detect scope drift against a saved baseline.
* **Safe Cleanup Workflows:** Preview exactly what will be deleted and why protected versions are kept before taking action.
* **Retention Policy Simulation:** Evaluate the impact of new retention limits before modifying actual feed settings.
* **Zero-Risk Operations:** Deletion is disabled by default, requires explicit manual confirmation (typing the package name), and deleted versions are recoverable from the Recycle Bin for 30 days.
* **Privacy-First Architecture:** Runs entirely within your browser/Azure DevOps context with no external backend server.

---

## 📦 Supported Feed Types

Package Sentinel natively supports all primary Azure Artifacts package formats:
* **NuGet**
* **npm**
* **Python (PyPI)**
* **Maven**
* **Universal Packages**

---

## 🔐 Permissions & Privacy

The extension requests the **Packaging (Read, Write, and Manage)** scope:
* **Read:** Used during automated scans, dashboards, and security audits.
* **Manage:** Used solely when you explicitly confirm a package/version deletion action.

> **Privacy Notice:** Package Sentinel has no external backend infrastructure. All calculations, rule evaluations, and comparisons are processed locally inside your browser.

---

## 🚀 Quick Start

1. Install **Package Sentinel** from the Azure DevOps Marketplace.
2. Navigate to your project in Azure DevOps; click the **Package Sentinel** item in the sidebar navigation.
3. Click **Run scan** to audit your feeds.
4. Go to **Settings** to customize baseline rules and approved user lists.

---

## 🛠 Detailed Features

### 1. Feed Security Audit
* Evaluates permissions and issues findings rated **HIGH**, **MEDIUM**, or **LOW** based on strict, deterministic rules.
* Flags broad permissions (e.g., granting "Valid Users" group Contributor rights).
* Cross-references Contributors and Owners against an approved list maintained by you.
* Detects unconfigured upstream sources, missing retention policies, and excessive owner count.
* Compares current feed access settings against a saved baseline snapshot to highlight unauthorized changes.

### 2. Package Lifecycle Dashboard
* Filter and sort packages by version count and elapsed time since the last publish event.
* Displays status badges including *Multiple versions*, *Outdated*, *Pre-release only*, and *Retention policy needs review*.
* **Safe Labeling Logic:** Packages with no recent publish activity are **never** labeled as "unused", recognizing that legacy package versions may still be actively pulled in production builds.

### 3. Retention Policy Analyzer
* Displays current feed retention rules (versions kept per package and max age of downloaded versions).
* Simulates new retention limits, listing exact packages and versions eligible for cleanup under the proposed rules.
* Respects view promotions—versions promoted to a view are automatically exempt from retention limits.
* *Read-only tool:* Actual feed settings must be applied via native Azure Artifacts settings.

### 4. Safe Cleanup Preview
* Categorizes discovered versions into *Selected for cleanup* and *Protected*.
* Displays a clear reason for every protected item (e.g., `Latest`, `Promoted to a view`, `Newest N`, `Recently downloaded`).
* Deletion requires manual enablement and explicit confirmation (typing the exact package name).
* Deleted items are sent to the Azure Artifacts Recycle Bin, allowing full restoration within **30 days**.

---

## 📄 Support & Policies

* **Publisher:** Radwan Almsora
* **Issues & Feature Requests:** Please file bug reports and feature requests directly via [GitHub Issues](#).
* **Q&A:** Ask questions in the Q&A section on the Azure DevOps Marketplace page.
* **License:** Refer to the LICENSE file for usage terms.
```

eof

Would you like me to add additional sections to the README, such as build instructions or a section explaining custom rule configurations?
