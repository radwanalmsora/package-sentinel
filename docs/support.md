# Support & Help Guide

Thank you for using **Package Sentinel: Security & Governance for Azure Artifacts**. We are dedicated to providing clear support channels to ensure you get the most out of the extension.

---

## 🔍 Frequently Asked Questions (FAQ)

<details>
<summary><b>Does Package Sentinel replace Azure Artifacts?</b></summary>
<p>No. Package Sentinel works alongside Azure Artifacts. It reads your current settings and configurations, evaluates them against rules you control, and helps you identify vulnerabilities and perform safe cleanup previews.</p>
</details>

<details>
<summary><b>Does this extension send my data to external servers?</b></summary>
<p>No. Package Sentinel has no external backend or server infrastructure. All processing, scans, rule evaluations, and preview renderings happen 100% locally inside your browser session using Azure DevOps REST APIs.</p>
</details>

<details>
<summary><b>Will Package Sentinel automatically delete my package versions?</b></summary>
<p>No. Deletion is completely manual and disabled by default. When enabled, it requires explicit confirmation (typing the exact package name). All deleted versions are moved to the Azure Artifacts Recycle Bin and remain recoverable for 30 days.</p>
</details>

<details>
<summary><b>Why is a package with no recent publishes not marked as "Unused"?</b></summary>
<p>Packages with no recent publish activity may still be actively downloaded and consumed by production builds every day. Package Sentinel never assumes a package is unused simply because it hasn't been published recently.</p>
</details>

---

## 🛠️ How to Get Help

### 1. Bug Reports & Feature Requests (GitHub Issues)
If you encounter a bug, unexpected behavior, or have a feature request:
* Check existing [GitHub Issues](#) to see if your topic has already been discussed.
* If not, create a **New Issue** using the appropriate template:
  * **Bug Report:** Include your Azure DevOps environment details (Cloud Services vs Server), steps to reproduce, and screenshots if applicable.
  * **Feature Request:** Describe the proposed feature, the problem it solves, and your use case.

### 2. General Questions & Discussions (Marketplace Q&A)
For general usage questions, configuration advice, or community inquiries:
* Visit the **Q&A** tab on our [Azure DevOps Marketplace listing](#).
* Submit your question to receive help from the author or other community members.

---

## 🔐 Security & Vulnerability Reporting

If you discover a potential security issue or vulnerability within Package Sentinel:
* **Do not** post security vulnerabilities publicly on GitHub Issues or Marketplace Q&A.
* Please submit a confidential report directly via GitHub Security Advisories or contact the publisher directly through the contact options on the publisher profile page (**Radwan Almsora**).

---

## 📜 Support Policy & SLAs

* **Scope of Support:** Support covers extension-specific functionalities, rule definitions, lifecycle dashboard behavior, and cleanup previews. Native Azure Artifacts issues (e.g., feed creation, network access, Azure DevOps outages) should be directed to [Microsoft Azure DevOps Support](https://azure.microsoft.com/en-us/support/devops/).
* **Response Time:** As an open extension, issues and questions are reviewed on a best-effort basis. Critical bugs affecting extension usability are prioritized.
