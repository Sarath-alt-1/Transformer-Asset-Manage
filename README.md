# Transformer Asset Manager

A ServiceNow scoped application for tracking industrial power transformers as configuration items — built as part of a hands-on ServiceNow developer portfolio, drawing directly on prior experience as a transformer design / CAD engineer.

## Status: In Progress 🚧

Core data model is underway. Automation and reporting are next.

- [x] Scoped application created — *Transformer Asset Manager*
- [x] `Transformer` table created, extending `[cmdb_ci / alm_asset — confirm which]`
- [ ] Custom transformer-specific fields (serial number, rated capacity, voltage class, manufacturer, transformer type, etc.)
- [ ] Flow Designer: maintenance-due automation
- [ ] Fleet health dashboard / reporting
- [ ] Screenshots and field reference added to this README

## Overview

Industrial transformers need scheduled maintenance, inspection history, and lifecycle visibility — the same asset-management problem ServiceNow's CMDB/Asset framework is built to solve. This app models each transformer as a configuration item so that:

- Every unit carries maintenance and inspection history
- Maintenance-due dates trigger automated notifications/tasks via Flow Designer
- A dashboard rolls up fleet health and upcoming maintenance at a glance

## Why This Project

Built to bridge a background in transformer design and instrumentation with ServiceNow development — an app that models a domain problem I understand firsthand, rather than a generic tutorial CMDB.

## Tech Stack

- ServiceNow scoped application (custom app, not Global)
- `Transformer` table extending `[cmdb_ci / alm_asset]`
- Flow Designer (planned — maintenance-due automation)
- Reporting / Performance Analytics (planned — fleet health dashboard)

## Data Model

`Transformer` extends `[cmdb_ci / alm_asset]`, inheriting standard fields (attestation status, checked in/out, business unit, company, assignment group) plus custom fields for transformer-specific attributes — full list to be added once finalized.

## Roadmap

1. Finalize and confirm custom fields on the `Transformer` table
2. Build Flow Designer maintenance-due automation
3. Build fleet health dashboard
4. Add screenshots, field reference, and script snippets to this README

## Author

**Sarath** — CAD Design Engineer transitioning into ServiceNow development.
Portfolio projects: [alert-to-incident-restapi](https://github.com/Sarath-alt-1/alert-to-incident-restapi) · [sims-incident-management](https://github.com/Sarath-alt-1/sims-incident-management)
