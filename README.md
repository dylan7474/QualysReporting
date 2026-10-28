# Platform Governance Portal

https://dylan7474.github.io/QualysReporting

A lightweight governance platform for managing asset ownership, reconciliation, risk acceptance, and vulnerability prioritisation.

## Overview

The Platform Governance Portal is designed to act as an authoritative asset governance layer between infrastructure discovery tools and operational reporting.

The system treats asset discovery data as an input source while maintaining an independent Asset Register that serves as the ownership source of truth.

The goal is to eliminate repeated asset classification, simplify monthly reconciliation, improve ownership accuracy, and generate actionable remediation plans.

---

## Core Principles

### Asset Register is Authoritative

Ownership decisions are maintained within the Asset Register.

Discovery data can suggest classifications but must never overwrite existing decisions automatically.

### Discovery Sources are Advisory

Discovery platforms are used for:

- Asset discovery
- Vulnerability discovery
- Metadata enrichment

Discovery data is not treated as authoritative ownership information.

### Review Once

Assets should only require manual review when:

- Newly discovered
- Missing
- Materially changed
- Ownership conflicts are detected

Previously approved decisions should be preserved.

### Exception-Based Governance

The system focuses on:

- New Assets
- Missing Assets
- Changed Assets
- Ownership Conflicts
- Expired Risk Acceptances

Rather than requiring a full estate review each reporting cycle.

---

## Features

### Asset Reconciliation

Compare current asset discovery data against the Asset Register.

Identify:

- Existing Assets
- New Assets
- Missing Assets
- Changed Assets
- Ownership Conflicts

### Asset Register

Maintain:

- Ownership
- Service Classification
- Environment
- Criticality
- Lifecycle Status

### Review Queue

Provide a workflow for:

- Approving assets
- Rejecting assets
- Reassigning ownership
- Retiring assets

### Risk Register

Support risk acceptance processes including:

- Acceptance Date
- Review Date
- Approved By
- Business Justification

### Reporting

Generate:

- Governance Reports
- Asset Ownership Reports
- Risk Reports
- Executive Summaries
- Action Plans

### Historical Analysis

Track changes over time including:

- Asset Growth
- Asset Ownership Trends
- Risk Trends
- Vulnerability Trends
- Remediation Progress

---

## Asset Lifecycle

```text
Discovery
    ↓
Review Queue
    ↓
Approved / Rejected
    ↓
Asset Register
    ↓
Reporting & Governance
