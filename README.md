# FutureWork Admin

Public frontend repository for the FutureWork administration web application.

## Status

Repository initialized. The administration application, Google sign-in integration, and backend connection are not deployed yet. This repository initialization does not provide access to student records.

## Planned architecture

- GitHub Pages: static web interface.
- Google Apps Script: authenticated API and synchronization, subject to integration tests.
- Google Sheets: existing sources and separately controlled operational data.

## Public repository boundary

Only reviewed application code and synthetic test fixtures may be committed here. Never commit student records, spreadsheet exports, tokens, passwords, private configuration, internal backend documents, or backups.

Authorization must be checked by the backend for every read, write, and export. Hiding interface controls is not authorization.

## Integration acceptance

Before real data is enabled, test Google sign-in with both personal and work accounts, server-side permissions, audit attribution, and access revocation. Keep production sources unchanged during testing.
