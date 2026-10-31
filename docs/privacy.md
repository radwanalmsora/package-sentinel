# Privacy Policy for Package Sentinel

**Last Updated:** October 31, 2026  
**Publisher:** Radwan Almsora  

---

## 🔒 Overview

**Package Sentinel: Security & Governance for Azure Artifacts** ("the Extension") is designed with a **privacy-first, client-side architecture**. We respect your privacy and are committed to protecting the confidentiality and security of your code, package metadata, and organization settings.

---

## 🌐 Data Collection and Processing

### 1. No External Data Transmission
Package Sentinel **does not collect, store, transmit, or process any data on external servers**. All scans, audits, evaluations, and visualizations are performed **100% locally within your web browser** using standard Azure DevOps SDKs and REST APIs.

* **No Analytics or Telemetry:** The Extension does not use third-party analytics tools, tracking scripts, or telemetry frameworks.
* **No External Servers:** The developer does not host backend servers, databases, or API endpoints that receive data from your Azure DevOps environment.

### 2. Azure DevOps API Usage
To provide its functionality, Package Sentinel requests temporary access to read and manage feed settings within your Azure DevOps organization:
* **Read Scope:** Reads feed access control lists (ACLs), package metadata, version histories, and retention rules to generate reports and previews.
* **Manage Scope:** Executes version deletion requests **only** when explicitly authorized and confirmed by you.

All authentication tokens, API requests, and responses remain strictly within your browser session and your Azure DevOps organization's boundary.

---

## 💾 Local Storage

The Extension uses your browser’s local storage (or Azure DevOps Extension Data Service) solely to store your personal configuration settings, including:
* Custom baseline snapshots for permission comparisons.
* Your approved lists of Feed Owners and Contributors.
* Custom audit rule preferences.

This data is stored locally within your environment and is never shared with third parties.

---

## 🛡️ Data Retention & Safety

* **Package Deletion Safety:** Package Sentinel does not automatically delete any data. All cleanups require explicit manual user confirmation.
* **Recycle Bin Protection:** Deleted package versions are moved to your Azure Artifacts Recycle Bin, where they can be fully recovered within 30 days according to native Azure DevOps retention policies.

---

## 📄 Changes to This Policy

We may update this Privacy Policy from time to time to reflect changes in the Extension's features or legal requirements. Updates will be documented directly in this repository and on the Azure DevOps Marketplace listing page.

---

## ✉️ Contact & Support

If you have any questions, concerns, or inquiries regarding this Privacy Policy or the security of the Extension, please open an issue in the **GitHub Issues** section of this repository or contact us via the Marketplace Q&A tab.
