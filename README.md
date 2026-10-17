# AltCheck Fixtures Repository (`huzyow155/alt-check-fixtures`)

This repository serves static HTTPS fixtures for auditing with the AltCheck intelligent contract on GenLayer Studionet (Preview).

## Fixtures

| File | Purpose | Expected Mode | Target Grade / Outcome |
| :--- | :--- | :--- | :--- |
| `good.html` | Clean, semantic, fully accessible | `FULL` | Grade A (Score ~100) |
| `bad.html` | Deliberately violates R1-R12 rules | `FULL` | Grade F (Multiple rule deductions) |
| `mixed.html` | Balanced clear & vague alt/link texts | `FULL` | Mixed model findings (CLEAR & VAGUE) |
| `fixed.html` | Remediated `bad.html` | `FULL` | Grade A/B (Significant verified delta) |
| `shell.html` | Empty SPA client shell (`<div id="root">`) | `SHELL_ONLY` | Grade `N/A` (Score -1) |
| `demo.html` | Live before/after demo path | `FULL` | Starts bad, updated to fixed |
| `data.json` | JSON payload (non-HTML) | N/A | Reverts: `not an html page` |
| `notes.txt` | Plain text payload (non-HTML) | N/A | Reverts: `not an html page` |
