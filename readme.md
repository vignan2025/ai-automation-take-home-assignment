# D2C Haircare COD RTO Optimization System

An AI-powered decision engine, WhatsApp workflow simulator, and executive dashboard built for evaluating Cash on Delivery (COD) orders, reducing Return to Origin (RTO) costs, and maximizing net financial margin for a D2C haircare brand.

---

## 🚀 Quick Start (Run in under 1 minute)

1. Clone or download this repository:
   ```bash
   git clone https://github.com/vignan2025/ai-automation-take-home-assignment.git
   ```
2. Open the `index.html` file in any standard browser (Google Chrome, Microsoft Edge, Safari, Firefox).
3. **No installation, Node.js dependencies, or servers required!** Everything runs directly in the browser.

---

## 📋 What This System Solves

We run a D2C haircare brand where **55% of orders are Cash on Delivery (COD)** with a **28% RTO rate**. Each RTO costs ₹169+ in forward/return shipping, handling, and product damages. 

This system dynamically routes incoming COD orders into 4 operational buckets:
1. **Ship As-Is:** Low risk, high quality address.
2. **Ship After Confirmation:** First-time buyers / moderate risk (WhatsApp confirmation flow).
3. **Nudge to Prepaid:** High RTO pincodes/history (offers ₹40 discount to convert online).
4. **Hold / Cancel:** Blocked fake names, invalid addresses, or extreme risk.

---

## 📑 Included Deliverables & Features

* **Morning Dashboard (Part 3):** Displays yesterday's total orders evaluated, 4-bucket distribution, estimated RTO savings (₹), lost margin from cancelled genuine orders, and total net financial impact.
* **Decision Engine Simulator (Part 1):** Real-time order evaluation balancing LLM text scoring (address completeness & fake name detection) with deterministic pincode rules. Includes live non-technical slider controls.
* **WhatsApp Flow Simulator (Part 2):** Interactive chat flow testing customer responses (`YES`, `NO`, Hinglish replies, 24h timeouts) along with the unit-economic math behind the ₹40 prepaid discount incentive.
* **Executive Business Memo (Part 4):** Comprehensive 1–2 page memorandum written for the founder reconciling the Head of Operations vs. Head of Marketing trade-offs with financial justification.

---

## 🛠️ Architectural Boundary: LLM vs. Code

| Functionality | Technology Used | Operational Justification |
| :--- | :--- | :--- |
| Address Quality & Completeness | **LLM (NLP)** | Parses unstructured Indian/Hinglish addresses, identifying missing house numbers or landmarks. |
| Fake Name Detection | **LLM / Regex** | Detects gibberish names like `"asdf"`, `"test"`, or keyboard mashing. |
| Pincode Historical RTO Lookup | **Deterministic Code** | Fast, exact database lookups ($O(1)$) of pincode RTO percentages. |
| Expected Profit & Threshold Math | **Simple Formula** | Pure mathematical calculations for margins, discounts, and net gain. |

---

## 📝 Submission Files Checklist

* `index.html` — Interactive Web Application (Dashboard, Simulator, WA Flow, & Executive Memo)
* `README.md` — Project setup and architecture documentation
* `Associate Software Engineer – Take-Home Assignment.pdf` — Assignment specification reference

---

### 📩 Contact & Developer Info
* **Role:** Associate Software Engineer Candidate
* **Repository:** [ai-automation-take-home-assignment](https://github.com/vignan2025/ai-automation-take-home-assignment)