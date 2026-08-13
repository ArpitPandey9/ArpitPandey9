# Arpit Pandey

I build research-grade data tools for digital assets, on-chain analytics, DeFi liquidity context, protocol risk, and reproducible crypto market-structure analysis.

My current focus is turning raw blockchain and market data into decision-useful research outputs: clear hypotheses, tested signals, benchmark-adjusted validation, documented limitations, and reproducible dashboards.

## Current flagship project

### Crypto Research Engine

An on-chain whale-flow research engine for crypto market structure, DeFi liquidity context, and benchmark-adjusted signal validation.

Repository: [crypto-research-engine](https://github.com/ArpitPandey9/crypto-research-engine)

What it does:

- detects and stores large on-chain transfer events
- normalizes token movement into USD-denominated whale-flow
- combines whale-flow with BTC/ETH market-price context
- validates signals against BTC benchmark-adjusted outcomes
- attaches event-time volatility and liquidity context
- summarizes outcome reliability through context-conditioned analysis
- presents results through a Streamlit research dashboard
- includes tests, CI, sample artifacts, and data-reproducibility documentation

Current local verification:

- 214 tests passing
- 91% total coverage
- conservative liquidity interpretation
- no fake data substitution
- no causality claim from transfers alone
- no financial-advice positioning

## Protocol verification case study

### WETH9 Large Deposits — Event-Level Verification

A separate fixed-window Ethereum investigation tests protocol execution directly rather than inferring behavior from a function selector alone.

For 135 successful native-ETH calls of at least 1,000 ETH to WETH9 between 23 Apr and 22 Jul 2026:

- 135 / 135 had exactly one matching WETH9 `Deposit` event
- 135 / 135 matched transaction value to the summed `Deposit`-event value in exact wei
- 135 / 135 matched transaction sender to `Deposit` destination
- 128 used selector-only calldata and 7 carried trailing calldata
- the 7 trailing-calldata cases grouped into 3 observed byte patterns with counts 5 / 1 / 1
- the analysis does not infer wallet software, entity ownership, shared infrastructure, or economic intent from those byte patterns

[Canonical row-level Dune evidence](https://dune.com/queries/8299357) · [Live Dune dashboard](https://dune.com/arpitpandey/weth9-large-deposits-event-level-verification) · [GitHub case study](https://github.com/ArpitPandey9/crypto-research-engine/blob/main/docs/WETH9_EVENT_LEVEL_VERIFICATION.md)

## Research notes

- [When Whale-Flow Fails](https://arpitpandey9.github.io/research/whale-flow-failure.html) — why positive ETH whale-flow should not be treated as a standalone durable signal after BTC benchmark adjustment.

## Research focus

- On-chain analytics
- DeFi liquidity and market depth
- Protocol and market-structure risk
- Blockchain intelligence workflows
- Benchmark-adjusted signal validation
- Data quality, auditability, and reproducibility
- Crypto research dashboards and evidence-based reporting

## Current research direction

I am currently exploring when whale-flow becomes decision-useful rather than noise.

The core research question:

> Under what market conditions does large on-chain whale-flow become useful after adjusting for broader crypto market movement?

The current project treats whale-flow as a testable hypothesis, not as proof of price impact.

## Portfolio principles

I try to build projects that are:

- honest about data limits
- reproducible from code and sample artifacts
- clear about what is tested versus what is assumed
- conservative with claims
- useful for research, risk, and analytics teams
- readable by both technical and financial audiences

## What I am building next

- event-time liquidity backfill for stronger DeFi liquidity context
- deeper protocol-risk and blockchain-intelligence case studies
- additional reproducible on-chain investigations with explicit evidence boundaries
- short research notes based on validated outputs

## Background

I work in financial operations and data-quality workflows, and I am building toward crypto research, on-chain analytics, protocol-risk, and digital-assets intelligence roles.

My edge is the combination of:

- financial-data discipline
- operational controls mindset
- Python-based analytics
- audit-oriented documentation
- crypto market-structure research
- reproducible public proof-of-work
