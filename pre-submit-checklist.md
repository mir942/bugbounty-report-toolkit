# Pre-submission checklist

## Scope
- [ ] Asset is listed in scope (or matches a listed wildcard)
- [ ] Vulnerability class is not on the out-of-scope list
- [ ] Read the program's policy and disclosed reports for duplicates

## Commonly ineligible or informative (check before filing)
- [ ] WordPress `/wp-json/wp/v2/users` enumeration (documented default behavior)
- [ ] Permissive CORS without demonstrated access to sensitive data
- [ ] Missing security headers, SPF/DMARC, or banner disclosure
- [ ] Clickjacking on pages with no sensitive actions
- [ ] Public-by-design data (public metadata, public API docs)
- [ ] Expired or misconfigured TLS with no further impact
- [ ] Automated scanner output with no manual proof of impact

## Report quality
- [ ] Reproducible steps that someone else can follow
- [ ] Impact stated honestly, including what was NOT accessed
- [ ] Severity matches the demonstrated impact
- [ ] Every claim ("verified in browser", etc.) is something I actually did
- [ ] No placeholders left (`<handle>`, `<target>`)
- [ ] Attachments contain only what the program needs

## Conduct
- [ ] Non-destructive requests only
- [ ] Own accounts only; stopped once behavior was confirmed
- [ ] Research header sent if the program requires one
