# Awesome-Automated-Intercompany-Reconciliation-Engines

# Top Automated Intercompany Reconciliation Engines Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Intercompany Matching, Netting & Global Consolidation*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Automated Intercompany Reconciliation Engines**. These tools enable corporate accounting teams to automate matching of cross-entity transactions, resolve mismatches, execute netting and settlement, and ensure accurate consolidation across global subsidiaries.

**Examples** include BlackLine, Trintech Cadency, FloQast, AutoRek, ReconArt, OneStream, Duco, SmartStream, HighRadius, and Adra by Trintech (the category leaders).

**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, deterministic matching engines, and open ERP-integrated reconciliation—ideal for finance teams, controllers, and developers seeking transparent, vendor-independent intercompany infrastructure.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[BlackLine](https://www.blackline.com/products/intercompany/)**
  Intercompany financial management platform with **Intercompany Create**, **Balance & Resolve**, and **Net & Settle** modules. Centralizes data from multiple ERPs into a global subledger, automates matching of intercompany transactions, enforces transfer pricing policies, and enables bilateral netting to reduce settlement transactions and bank fees. AI-powered predictive guidance improves transaction booking accuracy before posting to general ledger. Integrates with ERP and treasury systems for cash pooling and forecasting.

- **[Trintech Cadency](https://www.trintech.com/cadency/intercompany-accounting/)**
  Intercompany accounting automation with **Cadency Match** for transaction-level reconciliation. Achieves **90%+ auto-reconciliation** of intercompany transactions and **60%+ reduction in settlement time**. Features preventative and detective controls, multi-way matching, complex exception handling, and daily reconciliation capabilities. Purpose-built integrations bring detailed transactional data from any source. LKQ case study: executed 100+ acquisitions without increasing headcount, unified close tasks across all entities. Siemens reduced manual analysis from 15,000+ line items to fewer than 200 (99% reduction).

- **[FloQast Intercompany](https://www.floqast.com/)**
  AI-assisted intercompany automation that centralizes transactions and balances in one location. Features **AI-powered matching** that learns from manual matches, multi-currency conversion (local, functional, reporting currencies), and drill-through visibility into transactions behind each balance. Designed for quick deployment (days to weeks, not months). Accounting-centered AI keeps teams in control while reducing manual error-prone reconciliations.

- **[AutoRek](https://autorek.com/finance-reconciliations/)**
  Finance reconciliation platform automating balance sheet, bank, and intercompany reconciliations across entities and currencies. Features rule-based matching, real-time exception handling, configurable workflows with sign-off tracking, and complete audit trails with time-stamped records. Integrates with TMS, ERP, GL, and banking platforms. Achieves **100% match accuracy with over 99% match rates**. No-code configuration fully owned by operations.

- **[ReconArt](https://www.reconart.com/)**
  Financial reconciliation and close automation platform handling bank statements, intercompany transactions, and GL-to-subledger matching. **ReconArt Data Factory (RDF)** normalizes formats, currencies, and date conventions before matching. Rule-driven auto-matching processes high volumes instantly with exception classification and automated routing. Most clients reach **97–98% auto match rates** within a few reconciliation cycles. Supports CSV, XLSX, XML, BAI, ACH, SWIFT MT, camt.053, and custom formats.

- **[OneStream](https://www.onestream.com/)**
  Unified platform for financial close and consolidation replacing fragmented point solutions. **Transaction Matching (TXM)** automates high-volume reconciliations for intercompany, invoice-to-receipt, and corporate credit card transactions. **SensibleAI Account Reconciliations** detects anomalies and flags risks (unusual adjustments, missing documentation) early in the close. AI models learn from historical patterns to improve reconciliation policies, templates, and automation strategies. Average **54% time savings** for financial close and consolidation.

- **[Duco](https://www.duco.com/)**
  Cloud-native reconciliation platform with **Duco Cash** for intercompany matching. Uses **Text Equivalence rules** and reference tables to handle value mismatches (e.g., "O" matching "Option"). Generates **write-offs** and **netted transactions** when matching with amount differences within tolerance. Rule-driven matching with configurable tolerances, date ranges, and multi-field criteria. Breaking fields analysis identifies match failures for rule refinement.

- **[SmartStream Air](https://smart.stream/)**
  AI-enabled cloud reconciliation platform processing **10+ billion transactions monthly** for institutions including Deutsche Bank and HSBC. **Smart Agents** (agentic AI layer) triage breaks, gather data, validate across systems, and resolve end-to-end with human-in-the-loop approvals and complete audit trails. Adaptive matching engine combines rules-based logic with machine learning. **29x faster break resolution**, 70% reduction in manual workload, 30–60% improvement in resolution times.

- **[HighRadius](https://www.highradius.com/product/reconciliation-software/)**
  AI-powered reconciliation platform achieving **90% automated matching rate**. Agentic AI autonomously discovers matching patterns and clusters, reducing manual rule maintenance. Automated exception workflows route variances to correct owners with ML-suggested resolutions. **95% journal posting automation** closes the loop between reconciliation and GL. Integrates with 50+ ERPs, 10+ payment processors, and 100+ banks. 30% faster month-end close, 99% reconciliation accuracy.

- **[Adra by Trintech](https://www.trintech.com/)**
  Complete financial close automation platform with centralized checklists, automated multi-way transaction matching, and fast account reconciliations. **70% reduction in time spent matching transactions**, **67% reduction in time to close books**. System, source, and file-agnostic with flexible ERP integration. 3,500+ customers worldwide. Condado Tacos: $70K+ saved by avoiding full-time hire, 50% faster close across 28 stores.

## Open-Source GitHub Projects

- **[Matcha](https://github.com/Negentropy-Solutions/matcha)**
  Open-source payment reconciliation app for ERPNext (AGPLv3). Reconciles **Payment Entries** against **open invoices** with cross-company (XCO) support. Features reconcile workspace (company + date scoped), dashboard summary cards (unmatched payments, open invoices, overdue invoices, unmatched value), allocation tray with amount controls (one-to-many, split allocations, per-invoice adjustment), **FX gain/loss preview** before final reconciliation, and **cross-company reconciliation** that prepares and posts intercompany Journal Entries using bridge accounts. Exceptions tab for unmatched payments and ageing invoices. Full history and undo via **Matcha Payment Reconciliation Log**. Configuration via Matcha Settings with Intercompany Transfer Accounts per company. Frappe >=15.0.0, ERPNext, Python >=3.10.

- **[YARS (Yet Another Reconciliation System)](https://pkg.go.dev/github.com/aferryc/yars)**
  Financial reconciliation system for comparing internal transaction records with bank statements (MIT). Microservices architecture with API Server, Compiler Service, Reconciliation Service, PostgreSQL, Google Cloud Storage, and Kafka for event-driven communication. Features web UI for uploading transaction files (CSV), viewing summaries, and exploring unmatched transactions. Reconciliation service matches internal transactions with bank statements. Database schema includes transactions, bank_statements, recon_summary, unmatched_transactions, and unmatched_bank_statements. Docker and Docker Compose deployment. 4GB+ RAM recommended.

### Additional Strong Open-Source Options

- **[ERPNext](https://github.com/frappe/erpnext)** — Open-source ERP (GPL-3.0) with intercompany transactions, Journal Entry management, and multi-company consolidation. Foundation for Matcha reconciliation app.
- **[Odoo](https://github.com/odoo/odoo)** — Open-source business suite (LGPL-3.0) with multi-company accounting, intercompany rules, and automatic intercompany journal entries.
- **[OpenBoxes](https://github.com/openboxes/openboxes)** — Open-source supply chain management (EPL-1.0) with multi-location inventory tracking adaptable for intercompany goods transfers.
- Community **n8n** workflows for intercompany data extraction, matching automation, and exception alerting.

**Frameworks for building custom systems**: Combine **Matcha** for ERPNext-native intercompany reconciliation with **YARS** for bank statement matching, **ERPNext** or **Odoo** as the ERP backend, and **PostgreSQL** for persistence—creating a fully self-hosted, enterprise-grade intercompany reconciliation platform.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Intercompany reconciliation systems handling financial data must comply with accounting standards (GAAP, IFRS), tax regulations, and data protection requirements.
- **Intercompany reconciliation is more than matching balances.** It requires transaction-level detail, multi-currency handling, netting agreements, settlement execution, and elimination for consolidation. SaaS platforms like Trintech and BlackLine provide purpose-built modules for these workflows.
- **Open-source options are limited for enterprise intercompany.** Matcha addresses ERPNext payment reconciliation with XCO support—a significant step for open-source, but narrower than commercial intercompany suites. YARS handles bank statement matching, not full intercompany netting/settlement.
- Self-hosted open-source solutions require proper security hardening, ERP integration, and ongoing maintenance. Multi-entity consolidation and regulatory compliance remain the organization's responsibility regardless of tooling.

---

**Made for controllers, intercompany accountants, finance systems teams, and developers building transparent reconciliation solutions.**
Let's make Automated Intercompany Reconciliation more open, data-driven, and deterministic.
