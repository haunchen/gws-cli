---
"@googleworkspace/cli": patch
---

fix(setup): allow deselecting previously enabled APIs in `gws auth setup`

The API picker in `gws auth setup` marked already-enabled APIs as fixed
(non-toggleable), preventing users from reducing their enabled API set.
Now previously enabled APIs are pre-selected but can be deselected.
Deselected APIs are disabled via `gcloud services disable`.
