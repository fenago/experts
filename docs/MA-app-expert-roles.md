# Expert Roles for a GES M&A Decision-Support Application

*Prepared for Dr. Lee · November 19, 2026 · Companion to [GES-company-research.md](GES-company-research.md)*

> **Purpose:** Every role needed to build a world-class M&A application that helps GES executives evaluate acquisition targets. This list is tailored to GES: a private equity–backed trade show and experiential marketing company, owned by Truelink Capital, buying small agencies, contractors, and event-tech companies.
>
> **How to use this list:** You don't need to hire all of these people. Most are **subject-matter experts (SMEs)** whose knowledge you capture in the app's checklists, scoring models, and workflows. A few are **core team** members who build the app. The rest are **advisors** you consult for a few hours or days. Each role is tagged:
>
> - 🟢 **Core**: on the team building the product
> - 🟡 **Advisor**: ongoing part-time input (a few hours a month)
> - 🔵 **Consult**: one-time or occasional review

---

## 1. M&A and Business Strategy Experts

These people know *how deals actually get done*. They define the app's workflow and its scoring logic.

| # | Role | Why GES specifically needs it | What they shape in the app | Tag |
|---|---|---|---|---|
| 1 | **Corporate Development Lead** (former head of corp dev at a serial acquirer) | GES is running a buy-and-build strategy and needs a repeatable deal process | Deal pipeline stages, approval gates, deal-team roles, the overall process | 🟢 / 🟡 |
| 2 | **Private Equity Operating Partner** (buy-and-build specialist) | Truelink owns GES and judges every add-on by its exit value. The app must think the way the sponsor thinks | Exit-value math, multiple arbitrage (buying at 4x, owning at 6x+), add-on vs. platform logic, LP/board reporting | 🟡 |
| 3 | **Investment Banker / M&A Advisor** (lower-middle-market, buy and sell side) | Targets are small ($5M–$75M deals). Bankers know how auctions, IOIs, and LOIs work at that size | Deal timeline templates, IOI/LOI generators, process tracking, bid comparison | 🔵 |
| 4 | **Commercial Due Diligence Consultant** | GES's deals are justified by cross-selling. Someone has to test whether customers would actually buy more | Customer overlap analysis, cross-sell revenue model, market-sizing tools | 🔵 |
| 5 | **Business Development / Deal Sourcing Specialist** | The pipeline is the bottleneck. With 7,000+ U.S. exhibit companies, finding the right targets matters | Target database, sourcing workflow, outreach tracking, relationship CRM | 🟡 |

---

## 2. Industry (Domain) Experts: Live Events and Exhibitions

Generic M&A software misses what makes an events business valuable or risky. These experts make the app specific to GES.

| # | Role | Why GES specifically needs it | What they shape in the app | Tag |
|---|---|---|---|---|
| 6 | **Exhibition / General Service Contractor (GSC) Operations Expert** (e.g., a former Freeman, GES, or Shepard executive) | Contractor economics are unusual: show contracts, exclusive venue rights, freight and drayage, union labor, rental inventory | KPIs for contractor targets: show retention, revenue per square foot, contract renewal calendar, labor-cost ratio | 🟡 |
| 7 | **Experiential / Brand Agency Expert** | Spiro, 2Heads, and CSG are agencies. Agency value depends on people, retainers, and staff utilization | Agency KPIs: retainer vs. project mix, client concentration, staff utilization, key-person risk | 🟡 |
| 8 | **Association & Show Organizer Expert** (e.g., a former association executive or show director) | CSG's value is its association relationships, and organizers are GES's main buyers | Customer-value scoring, organizer relationship mapping, renewal-risk modeling | 🔵 |
| 9 | **Event Technology / SaaS Expert** | Data and AI targets (registration, lead retrieval, housing) need software metrics, not services metrics. This fits Truelink's data/AI thesis | SaaS metrics module: recurring revenue, churn, customer lifetime value, customer acquisition cost, tech-stack fit with Visit and onPeak | 🔵 |
| 10 | **Venue & Hospitality Expert** | GES now sells "venue services," and onPeak depends on hotel contracts | Venue and hotel contract risk fields, room-block exposure analysis | 🔵 |
| 11 | **International Markets Advisor** (EMEA, Middle East, India) | GES operates in the UK, Europe, the Middle East, and India, and 2Heads was a UK deal | Country-risk factors, currency handling, local-market comparables | 🔵 |

---

## 3. Financial and Analytical Experts

These experts define *the numbers*: what a target is worth and whether its earnings are real.

| # | Role | Why GES specifically needs it | What they shape in the app | Tag |
|---|---|---|---|---|
| 12 | **Valuation / Financial Modeling Analyst** (investment banking or PE background) | Executives need fast, consistent valuations across many small targets | Valuation engine: comparable multiples, DCF, LBO/accretion, pro-forma combined P&L, scenario sliders | 🟢 |
| 13 | **Quality of Earnings (QoE) / Transaction Services Accountant (CPA)** | Small founder-owned firms often have messy books and owner add-backs. Event revenue is lumpy and seasonal | EBITDA adjustment workflow, add-back tracker, normalized-earnings view, working-capital peg calculator | 🟡 |
| 14 | **M&A Tax Advisor** | Deal structure (asset vs. stock purchase, cross-border UK/EU/Canada deals) changes the true price | Tax-structure comparison tool, after-tax value calculator | 🔵 |
| 15 | **Debt Financing / Treasury Advisor** | GES is PE-backed and carries debt. Add-ons are often funded by the credit line, within covenant limits | Leverage and covenant checker: "Can we afford this deal under our credit agreement?" | 🔵 |
| 16 | **Synergy & FP&A (Financial Planning & Analysis) Analyst** | GES publicly promised cross-sell synergies, so the board will ask whether they happened | Synergy model at signing, then tracking of actual vs. plan after close | 🟡 |
| 17 | **Market Intelligence / Research Analyst** | Someone has to keep the target universe and competitor moves (Freeman, Fern/MSouth, Skyline) current | Market map, competitor deal tracker, news and ownership-change alerts | 🟢 |
| 18 | **Deal Structuring Specialist** (earn-outs, seller notes, rollover equity) | GES's own sale used a seller note, and founder deals usually include earn-outs to keep management | Earn-out and seller-note modeling, payout scenarios, management-retention economics | 🔵 |

---

## 4. Legal and Compliance Experts

Legal issues kill deals. These experts define the risk flags and diligence checklists.

| # | Role | Why GES specifically needs it | What they shape in the app | Tag |
|---|---|---|---|---|
| 19 | **M&A Transactional Attorney** | Purchase agreements, reps and warranties, indemnities, closing conditions | Legal diligence checklist, document request list (DRL), LOI and term-sheet templates, key-terms tracker | 🟡 |
| 20 | **Antitrust / Competition Counsel** | ⚠️ **Important for GES.** GES and Freeman dominate trade show general contracting. Buying a rival contractor could draw FTC/DOJ review (HSR filings) or UK/EU regulator attention | Antitrust risk flag on every target: market-share overlap, HSR filing-threshold check | 🔵 |
| 21 | **Labor & Employment Counsel** | ⚠️ **Critical for GES.** Show-floor labor is heavily unionized (Teamsters, IATSE, carpenters). Union agreements, pension obligations, WARN Act, and key-employee retention all affect value | Union and labor diligence module: collective bargaining agreements (CBAs), multi-employer pension liability, retention-agreement tracker | 🟡 |
| 22 | **Commercial Contracts Counsel** | ⚠️ **Critical for GES.** The value of contractors and agencies sits in show, venue, and client contracts. Change-of-control clauses can let customers walk away after a sale | Contract-review workflow: change-of-control flags, exclusivity terms, renewal dates (a strong use case for AI) | 🟡 |
| 23 | **Data Privacy & Cybersecurity Counsel** | Visit and onPeak hold attendee personal data. Event-tech targets bring GDPR (Europe), CCPA (California), and UK data-protection exposure | Privacy diligence checklist, data-flow risk scoring | 🔵 |
| 24 | **International / Cross-Border Counsel** (UK, EU, UAE, India, Canada) | Non-U.S. deals involve local corporate law, employment rules, and foreign-investment rules | Country-specific diligence checklists | 🔵 |
| 25 | **Anti-Corruption / Sanctions Compliance Specialist** (FCPA, UK Bribery Act) | GES operates in the Middle East and India, which are higher-risk regions for corruption issues | Compliance screening step for targets and their owners | 🔵 |
| 26 | **Intellectual Property Attorney** | Agencies own creative IP. Event-tech targets own software and patents | IP ownership checklist, open-source license review for tech targets | 🔵 |
| 27 | **R&W (Representations & Warranties) Insurance Broker** | R&W insurance is now standard in PE add-on deals and affects deal terms | Insurance cost and coverage fields in the deal model | 🔵 |

---

## 5. Operational Diligence and Integration Experts

Most M&A value is won or lost *after* the deal closes. GES has already used two integration models: folding 2Heads into Spiro, and running CSG as a standalone company.

| # | Role | Why GES specifically needs it | What they shape in the app | Tag |
|---|---|---|---|---|
| 28 | **Integration Management Office (IMO) Lead / Post-Merger Integration Expert** | GES plans many add-ons. Repeatable integration is the difference between a platform and a pile of companies | 100-day plan templates (fold-in vs. standalone), integration task tracker, milestone dashboards | 🟡 |
| 29 | **HR / People & Culture Diligence Specialist** | Agencies are only as good as their people. GES's model depends on keeping founders and teams | Key-person risk scoring, retention and compensation planning, culture assessment | 🔵 |
| 30 | **Compensation & Benefits / Earn-out Design Expert** | Keeping founders motivated after closing (CSG's Paige Cardwell, 2Heads' Paul Godwin) | Retention-package modeling linked to earn-outs | 🔵 |
| 31 | **IT & Systems Integration Diligence Expert** | Targets must connect to GES systems: the Expresso ordering portal, ERP, CRM, and Visit/onPeak platforms | IT diligence checklist, systems-compatibility scoring, integration cost estimates | 🔵 |
| 32 | **Cybersecurity Diligence Specialist** | Acquiring a breached company means inheriting its breach, which is especially risky for event-data companies | Cyber risk scorecard per target | 🔵 |
| 33 | **Operations / Supply Chain Diligence Expert** | Contractors and exhibit houses run warehouses, freight, fabrication shops, and rental inventory | Asset and inventory review, facility-overlap and consolidation analysis | 🔵 |
| 34 | **ESG / Sustainability Advisor** | Sustainability is a GES selling point (carpet recycling, reusable booths), and LPs increasingly ask about ESG | ESG diligence fields and scoring | 🔵 |
| 35 | **Enterprise Risk Manager / Insurance Specialist** | Event businesses carry liability, cancellation, and force-majeure risk (COVID nearly wiped out 2020 revenue) | Risk register, revenue-concentration and event-cancellation stress tests | 🔵 |

---

## 6. Product and Technology Team (Building the App)

These are the people who turn all of the expertise above into working software.

| # | Role | Responsibility | Tag |
|---|---|---|---|
| 36 | **Product Manager** (ideally with fintech or deal-software experience) | Turns expert knowledge into features, prioritizes, and runs user interviews with GES executives | 🟢 |
| 37 | **UX / Product Designer** | Executive dashboards: simple, decision-focused, mobile-friendly for busy executives | 🟢 |
| 38 | **Full-Stack Software Engineers** (2–3) | Build the application: pipeline, models, dashboards, workflows | 🟢 |
| 39 | **Data Engineer / Data Architect** | Connects data sources (PitchBook, Capital IQ, Crunchbase, trade publications, association directories, GES internal data) | 🟢 |
| 40 | **AI / ML Engineer** | LLM features: target sourcing, website and news summaries, contract clause extraction, data-room summarization, memo drafting | 🟢 |
| 41 | **Security & Compliance Engineer** | Deal data is highly confidential. Needs SSO, role-based access, audit logs, encryption, and likely SOC 2 | 🟢 / 🟡 |
| 42 | **QA / Test Engineer** | Valuation math must be exactly right, because executives make multimillion-dollar decisions on it | 🟢 |
| 43 | **Financial Model Validator** (independent reviewer) | Checks that the app's formulas match how bankers and auditors calculate | 🔵 |
| 44 | **Solutions Architect / DevOps Engineer** | Hosting, integrations with GES and Truelink IT, data residency (UK/EU data) | 🟡 |

---

## 7. Customer-Side Stakeholders (at GES and Truelink)

These people aren't hires. They are the **users and decision-makers** you need to interview and keep involved. Their needs define what "world-class" means.

| Stakeholder | What they need from the app |
|---|---|
| **CEO**, GES (Derek Linde) | Strategic fit at a glance, pipeline overview, go/no-go recommendations |
| **CFO**, GES | Valuation, financing capacity, synergy tracking, earnings impact |
| **General Counsel**, GES | Legal risk flags, diligence status, contract issues |
| **Operating company presidents** (Exhibitions, Spiro, onPeak, Visit, CSG) | Targets relevant to their business unit; integration ownership |
| **Head of Corporate Development** (if GES has one) | Day-to-day pipeline management; the primary power user |
| **Truelink deal partner** (Luke Myers) and deal team | Exit-value impact, portfolio-level reporting, board materials |
| **CHRO / HR leader** | People and retention risks, integration staffing |
| **CIO / IT leader** | Systems integration, security approval of the app itself |

---

## 8. Recommended Lean Starting Team

You can build an excellent first version without all 44 roles:

**Core build team (about 6–8 people)**
1. Product Manager
2. UX Designer
3. 2–3 Full-Stack Engineers
4. Data / AI Engineer
5. Valuation / Financial Modeling Analyst
6. Market Intelligence Analyst (part-time is fine at first)

**Standing advisory panel (a few hours a month each)**
1. Corporate Development / PE Operating Partner
2. Exhibition-industry operations expert (contractor side)
3. Agency M&A expert
4. QoE accountant (CPA)
5. M&A attorney
6. Labor & employment counsel (because of unions)
7. Post-merger integration lead

**Bring in as needed (one-time consults)**
Antitrust, tax, privacy, international counsel, cyber, ESG, and the other 🔵 roles. Consult them once to build the relevant checklist or module into the app, then again for periodic reviews.

> **Key idea:** The app *packages* these experts' judgment into scorecards, checklists, and models, so that GES executives get expert-level guidance on every deal without convening all of these specialists each time.

---

## 9. The Three GES-Specific Risks to Get Right

If you prioritize only three specialist areas beyond the core team, choose these. Generic M&A tools tend to miss them for a company like GES:

1. **Antitrust:** GES and Freeman form a near-duopoly in general contracting, so buying a rival contractor could trigger regulatory review.
2. **Union labor:** show-floor labor contracts and multi-employer pension liabilities can hide large costs.
3. **Change-of-control in show and venue contracts:** a contractor's value can disappear if its key shows can terminate after the sale.
