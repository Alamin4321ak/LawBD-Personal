# LawBD — Bangladesh Law & Lawyer Consultation Portal
### CSE Capstone Project: Client-Side Legal Information & Booking Architecture

A comprehensive, responsive, single-file web application providing access to **20 codified statutory laws of Bangladesh** and connecting citizens with **20 specialized chamber advocates and barristers** across distinct legal categories.

---

## 📌 Project Overview

**LawBD (AinSheba Portal)** is developed in pure HTML5, modern Vanilla CSS, and JavaScript. It serves as an academic-grade demonstration of:
1. **Curated Legal Compendium:** 20 fundamental Bangladesh acts with summarized provisions and direct links to official Ministry of Law ([bdlaws.minlaw.gov.bd](http://bdlaws.minlaw.gov.bd/)) enactments.
2. **Directory of 20 Advocates:** Covering 20 distinct legal practice areas with verifiable chambers (Supreme Court Bar Association, Motijheel C/A, Gulshan, Agrabad Chattogram), court admissions, contact details, and fee structures.
3. **Interactive Search & Filtering:** Dynamic, debounced search across statutes, categories, advocate names, and chamber locations.
4. **Client-Side Consultation Scheduler:** An appointment booking engine with validation for Bangladeshi contact numbers (`+880` / `01...`), pre-selected advocate links, conflict-free appointment ID generation (`BDL-2026-XXXX`), and a printable consultation pass.
5. **Session Persistence (Local Storage):** Simulates a consultation ledger using browser `localStorage` so evaluators and users can view, filter, review, and print their appointment vouchers without requiring a backend database.
6. **Statutory Litigation Tools:** Includes a court fee estimator based on the *Court Fees Act, 1870* and an emergency hotline directory (Government Legal Aid `16450`, Police `999`, ACC `106`, etc.).

---

## 📂 File Architecture

The entire portal is contained within a single standalone file for immediate portability:

```
LawBD/
├── index.html       # Complete application (Semantic HTML5, CSS design system, and JS logic)
└── README.md        # Technical documentation & project defense guide
```

> **Why Single-File Architecture?**  
> Enables instant zero-dependency execution across any modern browser (Chrome, Edge, Firefox, Safari) without requiring `node_modules`, bundling tools, or live web servers.

---

## ⚖️ 20 Indexed Bangladesh Laws

| # | Statute Name | Act / Year | Category | Official Source |
|---|---|---|---|---|
| 1 | The Constitution of the People's Republic of Bangladesh | 1972 (Supreme Law) | Constitutional | [bdlaws act-367](http://bdlaws.minlaw.gov.bd/act-367.html) |
| 2 | The Penal Code, 1860 | Act XLV of 1860 | Criminal | [bdlaws act-11](http://bdlaws.minlaw.gov.bd/act-11.html) |
| 3 | The Code of Criminal Procedure, 1898 (CrPC) | Act V of 1898 | Criminal | [bdlaws act-75](http://bdlaws.minlaw.gov.bd/act-75.html) |
| 4 | The Code of Civil Procedure, 1908 (CPC) | Act V of 1908 | Civil & Remedies | [bdlaws act-86](http://bdlaws.minlaw.gov.bd/act-86.html) |
| 5 | The Evidence Act, 1872 | Act I of 1872 | Civil & Remedies | [bdlaws act-24](http://bdlaws.minlaw.gov.bd/act-24.html) |
| 6 | The Contract Act, 1872 | Act IX of 1872 | Commercial & Corporate | [bdlaws act-26](http://bdlaws.minlaw.gov.bd/act-26.html) |
| 7 | The Transfer of Property Act, 1882 | Act IV of 1882 | Property & Land | [bdlaws act-48](http://bdlaws.minlaw.gov.bd/act-48.html) |
| 8 | The Specific Relief Act, 1877 | Act I of 1877 | Civil & Remedies | [bdlaws act-32](http://bdlaws.minlaw.gov.bd/act-32.html) |
| 9 | The Bangladesh Labor Act, 2006 | Act XLII of 2006 | Commercial & Corporate | [bdlaws act-952](http://bdlaws.minlaw.gov.bd/act-952.html) |
| 10 | The Companies Act, 1994 | Act XVIII of 1994 | Commercial & Corporate | [bdlaws act-787](http://bdlaws.minlaw.gov.bd/act-787.html) |
| 11 | The Negotiable Instruments Act, 1881 | Act XXVI of 1881 | Commercial & Corporate | [bdlaws act-43](http://bdlaws.minlaw.gov.bd/act-43.html) |
| 12 | Cyber Security Act, 2023 | Act 38 of 2023 | Tech & Public Safety | [bdlaws act-1445](http://bdlaws.minlaw.gov.bd/act-1445.html) |
| 13 | The Family Courts Act, 2023 | Act 51 of 2023 | Family | [bdlaws act-1458](http://bdlaws.minlaw.gov.bd/act-1458.html) |
| 14 | The Muslim Family Laws Ordinance, 1961 | Ordinance VIII of 1961 | Family | [bdlaws act-305](http://bdlaws.minlaw.gov.bd/act-305.html) |
| 15 | The Consumer Rights Protection Act, 2009 | Act XXVI of 2009 | Commercial & Corporate | [bdlaws act-1011](http://bdlaws.minlaw.gov.bd/act-1011.html) |
| 16 | The Anti-Corruption Commission Act, 2004 | Act V of 2004 | Criminal | [bdlaws act-906](http://bdlaws.minlaw.gov.bd/act-906.html) |
| 17 | The Right to Information Act, 2009 | Act XX of 2009 | Constitutional | [bdlaws act-1010](http://bdlaws.minlaw.gov.bd/act-1010.html) |
| 18 | The Bangladesh Environment Conservation Act, 1995 | Act I of 1995 | Tech & Public Safety | [bdlaws act-791](http://bdlaws.minlaw.gov.bd/act-791.html) |
| 19 | The Arbitration Act, 2001 | Act I of 2001 | Commercial & Corporate | [bdlaws act-840](http://bdlaws.minlaw.gov.bd/act-840.html) |
| 20 | The Narcotics Control Act, 2018 | Act 63 of 2018 | Tech & Public Safety | [bdlaws act-1262](http://bdlaws.minlaw.gov.bd/act-1262.html) |

---

## 👨‍⚖️ 20 Specialized Advocates & Chambers

Each profile represents a distinct branch of Bangladesh law:

1. **Barrister Rafiqul Islam** — Criminal Defense & Trial *(Supreme Court Bar Annex, Dhaka)*
2. **Barrister Tania Ahmed** — Corporate, M&A & Joint Ventures *(Concord Tower, Gulshan-2, Dhaka)*
3. **Advocate M. Shahidur Rahman** — Constitutional Law & Writ *(Purana Paltan Line, Dhaka)*
4. **Advocate Farzana Sharmin** — Family, Marriage & Custody *(Dhanmondi, Dhaka)*
5. **Advocate Mozammel Haque Bhuiyan** — Land Dispute & Title Suits *(Segunbagicha Law Chambers, Dhaka)*
6. **Barrister Tanvir Hasan** — Cyber Law & IT *(Banani, Dhaka)*
7. **Advocate Nazmul Karim Chowdhury** — Banking, Artha Rin & Cheque Dishonour *(Motijheel C/A, Dhaka)*
8. **Advocate Nasreen Sultana** — Labor & Industrial Employment *(Tejgaon Commercial Area, Dhaka)*
9. **Barrister K. M. Zillur Rahman** — Intellectual Property & Trademarks *(Uttara Model Town, Dhaka)*
10. **Advocate S. M. Rezaul Karim** — Taxation, VAT & Customs *(Kakrail, Dhaka)*
11. **Barrister Mahbub Alam** — Admiralty & Maritime Law *(Agrabad C/A, Chattogram)*
12. **Advocate Syeda Rizwana Akhter** — Environmental Law & Public Green Action *(Lalmatia, Dhaka)*
13. **Advocate Zahidul Islam** — Human Rights & Civil Liberties *(Bijoynagar, Dhaka)*
14. **Barrister Ashiqur Rahman** — Arbitration & ADR *(Mohakhali DOHS, Dhaka)*
15. **Advocate Dr. Sabrina Yasmin** — Medical Negligence & Health Law *(Mirpur DOHS, Dhaka)*
16. **Barrister Fariha Kabir** — Immigration & Foreign Visas *(Gulshan-1, Dhaka)*
17. **Advocate Anisur Rahman** — Media, Libel & Defamation *(Topkhana Road, Dhaka)*
18. **Advocate Kamrul Hasan** — Consumer Protection & Fair Trade *(Barishal / Segunbagicha)*
19. **Advocate Moniruzzaman Khan** — Insurance & Actuarial Risk *(Dilkusha C/A, Dhaka)*
20. **Barrister Saimon Farhad** — Telecommunications & Fintech Regulation *(Kawran Bazar, Dhaka)*

---

## 🔬 Frontend vs. Backend Distinction (CSE Note)

As noted in the project specification:
- **Client-Side Prototype (Current Implementation):**
  - Syntactic & semantic validation of form inputs (Regular Expression checks for Bangladeshi phone numbers `01[3-9]\d{8}`).
  - Dynamic UI state binding (auto-scrolling and pre-selecting an attorney from their card).
  - Persistence using the HTML5 `localStorage` API, permitting testing of booking lifecycles, cancellations, and printable slips.
- **Full-Stack Production Requirement (Future Roadmap):**
  - **Server-Side API:** A REST or GraphQL API (e.g., Express.js, FastAPI, or Laravel) to authenticate requests and mitigate spam/bot submissions.
  - **Database & Concurrency:** A relational database (PostgreSQL/MySQL) with ACID transactions to prevent double-booking of lawyer time slots.
  - **Authentication & Security:** JWT or session-based authentication with end-to-end encryption for sensitive case descriptions.
  - **Payment Gateway:** Integration with SSLCommerz, bKash, or Nagad for consultation retainer deposits.

---

## 🚀 How to Run

### Method 1: Direct File Execution (Recommended)
1. Open the project folder `c:\Users\User\Downloads\LawBD`.
2. Double-click [index.html](file:///c:/Users/User/Downloads/LawBD/index.html) in your file manager. It will open in Google Chrome, Microsoft Edge, or Mozilla Firefox.

### Method 2: Local HTTP Server (Python)
If you prefer running via a localhost server:
```powershell
cd c:\Users\User\Downloads\LawBD
python -m http.server 8000
```
Then visit: `http://localhost:8000/index.html` in your browser.

---

## 🎨 UI/UX Features
- **Dark & Light Mode:** Toggleable via header icon, with user preference saved in `localStorage`.
- **Responsive Layout:** Fluid CSS grid adapting from 360px mobile viewports to 4K desktop screens.
- **Print Optimization:** Formatted print styles (`@media print`) that format the booking slip as a clean consultation pass.
- **Zero Third-Party Dependency:** Built with vanilla web standards and inline vector SVGs, eliminating broken CDNs during offline evaluations.
