\<div align="center"\>
\<img src="[https://www.cmich.edu/Images/CMU-Seal-Maroon-1-Color-jpg.jpg](https://www.google.com/search?q=https://www.cmich.edu/Images/CMU-Seal-Maroon-1-Color-jpg.jpg)" alt="CMU Logo" width="150"/\>
\<h1\>🛡️ VAPT Report: Central Michigan University 🛡️\</h1\>
\<p\>
\<strong\>A comprehensive security assessment of CMU's public web infrastructure.\</strong\>
\</p\>

\<p\>
\<img src="[https://img.shields.io/badge/Assessment%20Date-August%202025-blue](https://www.google.com/search?q=https://img.shields.io/badge/Assessment%2520Date-August%25202025-blue)" alt="Assessment Date"\>
\<img src="[https://img.shields.io/badge/Report%20Version-1.1-informational](https://www.google.com/search?q=https://img.shields.io/badge/Report%2520Version-1.1-informational)" alt="Report Version"\>
\<img src="[https://img.shields.io/badge/Overall%20Risk-CRITICAL-red](https://www.google.com/search?q=https://img.shields.io/badge/Overall%2520Risk-CRITICAL-red)" alt="Overall Risk: CRITICAL"\>
\</p\>
\</div\>

-----

## 🚀 Overview

This repository contains the findings of a detailed **Vulnerability Assessment and Penetration Test (VAPT)** conducted on the internet-facing assets of Central Michigan University. The objective was to uncover and document security flaws that could pose a significant risk to the university's data, reputation, and operations.

The final deliverable is an interactive HTML report that provides in-depth analysis, contextual proofs-of-concept, and actionable remediation strategies.

### ➡️ **[View the Full HTML Report](https://www.google.com/search?q=./report1.html)** ⬅️

-----

## ✨ Key Features of the Report

✅ **Executive Summary:** A non-technical overview for stakeholders, highlighting the overall risk posture and strategic recommendations.

✅ **Interactive Findings:** A detailed breakdown of all 24 identified vulnerabilities, complete with:

  - **Severity & CVSS Scores:** Clear risk prioritization from `Informational` to `Critical`.
  - **OWASP/CWE Mapping:** Alignment with industry-standard security frameworks.
  - **Embedded PoCs:** Inline screenshots demonstrating exploitability.
  - **Targeted Remediation:** Step-by-step guidance to patch vulnerabilities.

✅ **Technology & Scope:** A comprehensive list of assessed targets and technologies identified during reconnaissance.

✅ **Modern & Readable UI:** A clean, well-structured HTML document for easy navigation and review.

-----

## 📊 Findings at a Glance

The assessment uncovered critical flaws that require immediate attention. The distribution of findings by severity is as follows:

| Severity      | Count |
|---------------|:-----:|
| 🔴 **Critical** | 5     |
| 🟠 **High** | 8     |
| 🟡 **Medium** | 6     |
| 🔵 **Low** | 3     |
| ⚪ **Informational**| 2     |

### ‼️ Highlighted Critical Vulnerabilities

  * **Remote Code Execution** via Log4Shell (`CVE-2021-44228`)
  * **Subdomain Takeover** via Dangling S3 DNS Record
  * **Chained Exploit** leading to RCE on `cmichmaestro.cmich.edu`
  * **Server-Side Template Injection** on FileSender instances
  * **Buffer Overflow** in an outdated Nginx 1.6.2 server

-----

## 🛠️ Methodology & Tools

The assessment employed a hybrid approach, combining automated scanning with in-depth manual testing to ensure comprehensive coverage and accuracy.

  - **Reconnaissance:** `Nmap`, `subfinder`
  - **Scanning & Analysis:** `Burp Suite Professional`
  - **Exploitation:** Custom Python Scripts, `Metasploit Framework`
  - **Reporting:** Custom HTML/CSS template

\<details\>
\<summary\>\<strong\>Click to view full Scope of Assessment\</strong\>\</summary\>

  - `cbalab.cmich.edu`
  - `cmichmaestro.cmich.edu`
  - `filesender.se.cmich.edu`
  - `d175137.dynamic.cmich.edu`
  - `bline.cmich.edu`
  - `dar.cmich.edu`
  - `apps.cmich.edu`
  - `cdn.cmich.edu`
  - `archive.applymed.cmich.edu`
  - `aux-helium.cmich.edu`
  - `blogs.cmich.edu`
  - `blackboard.cmich.edu`
  - `mirror.cmich.edu`
  - `libapps.cmich.edu`
  - `www.cmich.edu`
  - `galaxy.phy.cmich.edu`
  - `francesa.phy.cmich.edu`

\</details\>

-----

## 📖 How To Use

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/your-username/CMU-VAPT-Report.git
    ```

2.  **Navigate to the directory:**

    ```bash
    cd CMU-VAPT-Report
    ```

3.  **Open the report file:**

      - Open `report1.html` in any modern web browser (Chrome, Firefox, Edge).

4.  **Action the findings:**

      - Review the **Executive Summary** for a strategic overview.
      - Prioritize remediation based on the **Critical** and **High** severity vulnerabilities.
      - Share relevant sections with development and IT infrastructure teams to implement the recommended fixes.