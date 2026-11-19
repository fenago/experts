# GES M&A Expert Agents: User Guide

*Prepared for Dr. Lee · November 19, 2026*

This repository includes **15 Claude Code subagents** in `.claude/agents/`. Each one plays an expert role from [MA-app-expert-roles.md](MA-app-expert-roles.md). Anyone who opens this repo in Claude Code gets them automatically.

## The 15 agents

| # | Agent | Role | Group |
|---|---|---|---|
| 1 | `corp-dev-lead` | Head of Corporate Development. **Start here.** Frames the deal, routes questions to specialists, and writes the investment committee (IC) memo | M&A strategy |
| 2 | `pe-operating-partner` | Thinks like Truelink: exit value, multiple arbitrage, buy-and-build | M&A strategy |
| 3 | `commercial-diligence-consultant` | Market, customers, and validating the cross-sell thesis | M&A strategy |
| 4 | `exhibition-industry-expert` | Trade show contractor (GSC) operations: shows, labor, assets | Industry |
| 5 | `agency-ma-expert` | Experiential, creative, and association agencies (the Spiro/2Heads/CSG models) | Industry |
| 6 | `event-tech-expert` | Event software and data (fit with Visit and onPeak) | Industry |
| 7 | `market-intelligence-analyst` | Finds and scores targets, maintains the pipeline, profiles targets, maps the market, tracks competitors | Analyst |
| 8 | `valuation-analyst` | Valuation range, offer/walk-away prices, deal structure | Financial |
| 9 | `qoe-accountant` | Quality of Earnings: are the earnings real? | Financial |
| 10 | `synergy-analyst` | Cost and revenue synergies, plus post-close tracking | Financial |
| 11 | `ma-attorney` | Legal diligence, LOI/purchase agreement terms, IP, privacy | Legal |
| 12 | `antitrust-counsel` | Competition risk (GES and Freeman dominate GSC services), merger filings | Legal |
| 13 | `labor-employment-counsel` | Unions, pension withdrawal liability, WARN/TUPE, retention | Legal |
| 14 | `commercial-contracts-counsel` | Change-of-control clauses, show/venue contracts, revenue at risk | Legal |
| 15 | `integration-lead` | Post-merger integration: fold-in vs. standalone, 100-day plan | Integration |

## How to use them

Claude Code delegates to them automatically based on each agent's description. You can also call one explicitly:

```text
Use the corp-dev-lead agent to evaluate Acme Exhibits as an acquisition target for GES.
```

```text
@valuation-analyst value Acme Exhibits using the financials in docs/deals/acme-exhibits/
```

```text
Have the antitrust-counsel and labor-employment-counsel agents review Acme Exhibits in parallel.
```

To run a whole session as one agent:

```bash
claude --agent corp-dev-lead
```

## Where the work goes

Every agent reads `docs/GES-company-research.md` for context and writes its output into a shared deal folder, so the specialists build on each other's findings:

```text
docs/
├── GES-company-research.md     ← shared company context
├── market/                     ← market maps, competitor moves
├── pipeline/                   ← target lists, master pipeline
└── deals/<target-slug>/
    ├── target-profile.md       ← market-intelligence-analyst
    ├── qoe.md                  ← qoe-accountant
    ├── valuation.md            ← valuation-analyst
    ├── synergies.md            ← synergy-analyst
    ├── legal-diligence.md      ← ma-attorney
    ├── antitrust.md            ← antitrust-counsel
    ├── ...                     ← other specialists
    └── ic-memo.md              ← corp-dev-lead (final recommendation)
```

## A typical deal workflow

1. `market-intelligence-analyst` builds a ranked target list
2. `market-intelligence-analyst` profiles the top targets
3. `corp-dev-lead` frames the deal and picks which specialists to involve
4. Specialists run in parallel: industry expert, QoE, commercial, legal, antitrust, labor, contracts
5. `valuation-analyst` and `synergy-analyst` turn the findings into price and value
6. `pe-operating-partner` tests the deal against Truelink's exit thesis
7. `integration-lead` drafts the 100-day plan
8. `corp-dev-lead` writes the IC memo with a recommendation

## Important

These agents support executive decisions. They are **not** licensed attorneys, CPAs, or financial advisors. The legal and accounting agents flag items that need sign-off from licensed professionals. All research uses public information only; the agents never contact targets or customers.
