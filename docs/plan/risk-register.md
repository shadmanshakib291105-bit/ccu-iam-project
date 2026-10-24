# Risk register

Score = Likelihood (L) x Impact (I), each from 1 to 5. Ratings: Low 1-4, Medium 5-9, High 10-16, Extreme 20-25.
Each risk is also logged as a GitHub issue with the `risk` label.

| ID | Risk (cause -> effect) | L | I | Score | Strategy | Mitigation and contingency | Trigger | Owner |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| R1 | Core banking supports only legacy authentication -> SSO cannot be applied | 3 | 5 | 15 High | Mitigate | Core banking SSO shown in vendor proof of concept; fallback access gateway with MFA | PoC fails core banking scenario | IAM Architect |
| R2 | HR records inaccurate -> wrong access granted or leavers missed | 4 | 4 | 16 High | Mitigate | Data clean-up in audit; provisioning in report-only mode for 2 weeks | Reconciliation errors above 2% | HR systems lead |
| R3 | Staff unfamiliar with MFA -> lockouts in branches | 4 | 3 | 12 High | Mitigate | Pilot, e-learning, floor-walkers, self-service recovery | Lockout tickets above 30 per day | Change, Comms and Config Lead |
| R4 | Key client staff pulled into BAU -> delays | 3 | 4 | 12 High | Mitigate | Backfill budget, named deputies | Two missed workshops in a row | PM |
| R5 | Pen test finds critical issues late -> go-live postponed | 3 | 4 | 12 High | Mitigate | Security design review at M1; configuration scanning; 5 days float | Critical finding open at 30 June | Security Analyst |
| R6 | Extra applications requested -> scope creep | 4 | 3 | 12 High | Avoid | Change control; Phase 2 backlog | Change requests adding applications | PM |
| R7 | Admin access lost during PAM cut-over | 2 | 5 | 10 High | Mitigate | Tested break-glass accounts; staged onboarding; rollback plan | Failed break-glass test | Security Analyst |
| R8 | Licence or vendor delay -> build starts late | 3 | 3 | 9 Medium | Transfer | Contract milestones and penalties | Contract not signed by 18 Mar | PM |
| R9 | Integration effort underestimated -> cost overrun | 3 | 3 | 9 Medium | Transfer, mitigate | Fixed-price statement of work; 10% contingency | CPI below 0.95 | PM |
| R10 | Cloud IdP outage -> staff cannot log in | 2 | 5 | 10 High | Mitigate | 99.9% SLA; offline MFA; outage runbook | Vendor incident alert | Integration and Test Lead |
| R11 | Identity data stored offshore -> privacy breach | 2 | 4 | 8 Medium | Avoid | Australian region in contract; privacy impact assessment | PIA high finding | Security Analyst |
| R12 | MFA fatigue phishing during rollout -> account takeover | 3 | 4 | 12 High | Mitigate | Number matching, FIDO2 keys for admins, awareness messages | MFA denial spikes | Security Analyst |
