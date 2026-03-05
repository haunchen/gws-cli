---
"@googleworkspace/cli": patch
---

Fix auth deadlock when legacy credentials.enc exists without accounts.json: resolve_account now falls back gracefully instead of bailing, and login warns when email fetch fails
