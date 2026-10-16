# CVSS 4.0 notes for common web findings

Base metrics: AV, AC, AT, PR, UI, VC, VI, VA, SC, SI, SA.

## Choosing the less obvious metrics
- **AT (Attack Requirements):** use *Present* when exploitation depends on conditions the attacker doesn't control (for example, a victim holding a credential that may not exist). Use *None* only if the attack works in essentially every deployment.
- **UI:** *Passive* = the victim just loads attacker content. *Active* = the victim must take a deliberate action.
- **VC/VI/VA:** rate what you actually demonstrated. If you accessed nothing, don't choose High.
- **SC/SI/SA:** *None* unless impact clearly crosses into a different system.

## Example: permissive CORS (reflected Origin + credentials), no cookie auth
`CVSS:4.0/AV:N/AC:L/AT:P/PR:N/UI:P/VC:L/VI:N/VA:N/SC:N/SI:N/SA:N`
Scored Low (2.3) in HackerOne's calculator. Low is honest because no ambient credential exists.

## Rules of thumb
- Always let the platform's calculator produce the final score.
- Make the severity label in the report text match the calculator.
- Never raise a metric to reach a "better" rating.
