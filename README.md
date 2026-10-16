# Bug Bounty Report Toolkit

Templates and checklists for writing accurate, honest vulnerability reports for bug bounty programs and VDPs. Built from lessons learned while learning to triage my own findings before submitting them.

## What's inside
| File | Purpose |
|---|---|
| `report-template.md` | Report structure: Summary, Steps, Impact, Remediation, Testing notes |
| `cvss4-notes.md` | How I choose CVSS 4.0 metrics for common low-impact web findings |
| `pre-submit-checklist.md` | Checks to run before filing, including commonly ineligible finding types |

## Principles
1. **Scope first.** Confirm the asset is in scope and read the out-of-scope list before writing anything.
2. **Impact must be demonstrated, not hypothesized.** "If X were added later" is a hardening note, not an exploit.
3. **Never overclaim.** State plainly what you did not access or verify.
4. **Stay non-destructive.** Minimal requests, own accounts only, stop once the behavior is confirmed.
5. **Check for duplicates and disclosed reports** before spending effort on a write-up.

## Disclaimer
For authorized testing only. Only test assets that a program's policy explicitly puts in scope. No real targets, employee data or program-confidential details are included in this repo.

## Author
**Md Jahidul Mir**, Penetration Tester at TP-Link (web/mobile applications and cloud).
[LinkedIn](https://www.linkedin.com/in/mir942) · [GitHub](https://github.com/mir942)

This is a personal project. It is not affiliated with or endorsed by my employer, and the views here are my own.
