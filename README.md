# FutureWork Admin

Administration frontend: https://depocen-cased.github.io/fw-dev/

## Authentication

The page starts at an application-account login screen. Google sign-in is not required for operators. The server verifies the password and creates an expiring, revocable session. Report and identity records are fetched only after server authentication; the public frontend contains no account password, password hash, bearer token or record fixture.

## Current status

Local-account login, protected synthetic-data loading, test Sheet reading, test audit and logout have been exercised in the browser. Production source readers, identity decisions and Google Sheets report publishing are not enabled. Sample actions remain demonstrations.

Reports have separate attendance, assignment and session-summary views. A fixed output workbook has been initialized privately; no student records are published here.

## Public repository boundary

Commit reviewed frontend code only. Do not commit credentials, source spreadsheet IDs, student records, exports, internal backend documentation or backups. GitHub Pages publishes main/root automatically. Backend authorization is required for every data operation. A shared account identifies the account, not an individual colleague.
