# Open Component Lens v3.1 Pro 🔬⚡

An encrypted, serverless electronic component inventory, project tracker, and **Gemini AI** lab assistant designed for hardware hackers, makers, and embedded engineers.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Version](https://img.shields.io/badge/version-v3.1%20Pro-emerald.svg)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.x-38bdf8.svg)
![Gemini AI](https://img.shields.io/badge/AI-Gemini%201.5%20Flash-8e44ad.svg)

---

## 🌟 Key Features

* **🔍 AI-Powered Lens Scanner:** Snap or upload component photos. Powered by **Gemini 1.5 Flash**, it automatically extracts part numbers, operational voltage ranges ($V_{\min} - V_{\max}$), datasheets, and categories.
* **⚠️ Dynamic Stock Shortage Engine:** Real-time inventory monitoring that cross-references active project demands against current stock quantities.
* **🛠️ Isolated Project Playground:** Dedicated workspace per project build featuring checklist tasks, linked components, and a custom Gemini AI Lab Coach.
* **🔒 Enterprise-Grade Client-Side Security:** Zero backend database needed. Secrets (Gemini API keys, cloud master tokens) are encrypted locally using **AES-256** secured with a Master PIN.
* **☁️ Cloud Sync & Persistent Storage:** Seamless REST integration with JSONBin for multi-device sync without setup hassle.
* **🎨 Modern Tech-Focused Glassmorphism UI:** Built with dark-mode aesthetic, responsive layouts, and industry-standard typography for high legibility in lab environments.

---

## 🛠️ Architecture Overview

```
+-----------------------------------------------------------------+
|                       Open Component Lens                       |
+-----------------------------------------------------------------+
          |                                       |
   [ Client-Side AES-256 ]                 [ AI Lens Engine ]
   (Master PIN Encryption)                 (Gemini 1.5 Flash API)
          |                                       |
   [ JSONBin REST Sync ]                  [ Webcam / File Stream ]
```

---

## 🚀 Quick Start

Since **Open Component Lens** is fully client-side and serverless, no node server or build pipeline is strictly required to run it locally.

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/open-component-lens.git
cd open-component-lens
```

### 2. Run the App
Simply open `index.html` in your favorite web browser or start a lightweight HTTP server:

```bash
# Using Python
python3 -m http.server 8000

# Using Node.js serve
npx serve .
```

Navigate to `http://localhost:8000`.

---

## 📜 License, Legal Notice & Ethical Compliance

### 🔓 Open-Source Licensing
This project is open-source software licensed under the **MIT License**.
See the [LICENSE](./LICENSE) file for full terms. You are free to use,
modify, and distribute this software, including in proprietary or
closed-source projects, provided the original copyright and license
notice are retained.

---

### ⚠️ Strict Legal Notice & Terms of Use

> **CRITICAL DISCLAIMER:** This repository contains radio frequency (RF)
> analysis, packet injection, and wireless auditing tools. They are
> intended **strictly for authorized educational instruction, security
> research, penetration testing, and isolated laboratory use.**

By accessing, cloning, compiling, or deploying any part of this
software, you agree to the following:

1. **Mandatory Explicit Authorization** — You must obtain **explicit,
   written, and verifiable permission** from the system owner, network
   administrator, and (where applicable) facility management *before*
   performing any active wireless analysis, scanning, mapping, or
   security testing on any network or device you do not personally own.

2. **Lawful Use Only** — This software must not be used to target,
   disrupt, exploit, or intercept communications on networks or
   infrastructure without prior authorization. Laws governing wireless
   interception, jamming, deauthentication attacks, and unauthorized
   access **vary by country** and may include (depending on
   jurisdiction) computer-misuse laws, wiretap/interception statutes,
   and radio-frequency regulations enforced by bodies such as the FCC
   (United States), ETSI/national regulators (EU), Ofcom (UK), or
   equivalent authorities elsewhere. It is your responsibility to know
   and follow the laws that apply to you.

3. **Export Control Notice** — Software involving RF/wireless security
   tooling may be subject to export control or dual-use regulations in
   some countries (e.g., U.S. EAR, Wassenaar Arrangement-aligned
   regimes). Users are responsible for complying with any export or
   import restrictions that apply in their jurisdiction.

4. **User Responsibility** — The authors, developers, and contributors
   accept **no legal or financial liability** for any misuse, damage, or
   legal consequences arising from use of this software. The end user
   assumes full responsibility for their own actions and compliance
   with applicable law. (Note: some jurisdictions limit how far
   liability can be disclaimed by law — this notice does not override
   those protections where they apply.)

5. **"As-Is" Warranty Disclaimer** — This software is provided *"as is"*,
   without warranty of any kind, express or implied, including but not
   limited to warranties of merchantability, fitness for a particular
   purpose, and non-infringement. In no event shall the authors or
   copyright holders be liable for any claim, damages, or other
   liability arising from the software or its use.

6. **Contributions** — By submitting a pull request or other
   contribution, you confirm you have the right to submit the code and
   agree it will be licensed under the same terms as this project.

---

### 🛡️ Ethical Hacking Code of Conduct

- **Respect Privacy** — Never capture, store, or exfiltrate data
  belonging to uninvolved third parties.
- **Minimize Disruption** — Perform active testing only inside isolated
  lab environments (e.g., Faraday enclosures) or on systems you are
  explicitly authorized to test.
- **Responsible Disclosure** — If vulnerabilities are found during
  authorized testing, report them to the system owner through proper,
  formal channels — not publicly, until the owner has had a chance to
  remediate.
