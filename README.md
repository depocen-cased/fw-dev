# FutureWork Admin

Public frontend repository for the FutureWork administration web application.

## Status

Synthetic interface prototype is live at https://depocen-cased.github.io/fw-dev/. It includes a sample identity review queue, report filters, CSV export and in-memory demonstration history. All records are fictional and all sample changes reset on reload.

Google sign-in and backend are not configured or deployed. The sign-in button reports this explicitly. No student records or source spreadsheets are connected. Local backend tests are not evidence of successful real Google login.

## Planned architecture

- GitHub Pages: static web interface, currently main/root with automatic publication on commits.
- Google Apps Script: authenticated API and synchronization, subject to real integration tests.
- Google Sheets: existing sources and separately controlled operational data.

## Public repository boundary

Only reviewed application code and synthetic test fixtures may be committed here. Never commit student records, spreadsheet exports, tokens, passwords, private configuration, internal backend documents, or backups.

Authorization must be checked by the backend for every read, write, and export. Hiding interface controls is not authorization.

## Integration acceptance

Before real data is enabled, test Google sign-in with both personal and work accounts, server-side permissions, audit attribution, browser transport and access revocation. Keep production sources unchanged during testing.
