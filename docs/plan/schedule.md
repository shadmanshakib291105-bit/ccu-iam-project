# Project schedule (baseline)

Working days Monday to Friday, excluding NSW public holidays. All dependencies are finish-to-start. Project duration: 157 working days (1 Feb 2027 to 13 Sep 2027).

| ID | Activity | Duration (days) | Predecessors | Start | Finish | Total float | Critical |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1.1 | Approve project charter | 5 | - | 2027-02-01 | 2027-02-05 | 0 | Yes |
| 1.2 | Stakeholder analysis and register | 3 | 1.1 | 2027-02-08 | 2027-02-10 | 0 | Yes |
| 1.3 | Kick-off workshop | 1 | 1.2 | 2027-02-11 | 2027-02-11 | 0 | Yes |
| 2.1 | Current-state identity audit | 10 | 1.3 | 2027-02-12 | 2027-02-25 | 15 | No |
| 2.2 | Requirements and CPS 234 gap analysis | 10 | 1.3 | 2027-02-12 | 2027-02-25 | 0 | Yes |
| 2.3 | Vendor evaluation and selection | 15 | 2.2 | 2027-02-26 | 2027-03-18 | 0 | Yes |
| 2.4 | Solution architecture and role model | 15 | 2.1,2.3 | 2027-03-19 | 2027-04-12 | 0 | Yes |
| M1 | Design approval gate | 0 | 2.4 | 2027-04-12 | 2027-04-12 | 0 | Yes |
| 3.1 | Provision cloud tenant and test environment | 5 | M1 | 2027-04-13 | 2027-04-19 | 0 | Yes |
| 3.2 | HR-driven provisioning (joiner-mover-leaver) | 15 | 3.1 | 2027-04-20 | 2027-05-11 | 0 | Yes |
| 3.3 | SSO and phishing-resistant MFA | 10 | 3.1 | 2027-04-20 | 2027-05-04 | 5 | No |
| 3.4 | Privileged access management (PAM) vault | 15 | 3.1 | 2027-04-20 | 2027-05-11 | 20 | No |
| 3.5 | Application integrations | 20 | 3.2,3.3 | 2027-05-12 | 2027-06-08 | 0 | Yes |
| 4.1 | System integration testing | 10 | 3.4,3.5 | 2027-06-09 | 2027-06-23 | 0 | Yes |
| 4.2 | Penetration test and security review | 10 | 4.1 | 2027-06-24 | 2027-07-07 | 5 | No |
| 4.3 | User acceptance testing | 10 | 4.1 | 2027-06-24 | 2027-07-07 | 0 | Yes |
| M2 | Go-live approval (CAB) | 0 | 4.2,4.3 | 2027-07-07 | 2027-07-07 | 5 | No |
| 5.1 | Pilot rollout (head office, 150 users) | 10 | M2 | 2027-07-08 | 2027-07-21 | 5 | No |
| 5.2 | Training and communications | 15 | 4.3 | 2027-07-08 | 2027-07-28 | 0 | Yes |
| 5.3 | Phased rollout to 28 branches | 15 | 5.1,5.2 | 2027-07-29 | 2027-08-18 | 0 | Yes |
| 5.4 | Decommission legacy authentication | 5 | 5.3 | 2027-08-19 | 2027-08-25 | 5 | No |
| 6.1 | Hypercare | 10 | 5.3 | 2027-08-19 | 2027-09-01 | 0 | Yes |
| 6.2 | Handover to BAU operations | 5 | 6.1,5.4 | 2027-09-02 | 2027-09-08 | 0 | Yes |
| 6.3 | Lessons learned and closure report | 3 | 6.2 | 2027-09-09 | 2027-09-13 | 0 | Yes |
| M3 | Project closed | 0 | 6.3 | 2027-09-13 | 2027-09-13 | 0 | Yes |

Critical path: 1.1 > 1.2 > 1.3 > 2.2 > 2.3 > 2.4 > M1 > 3.1 > 3.2 > 3.5 > 4.1 > 4.3 > 5.2 > 5.3 > 6.1 > 6.2 > 6.3 > M3

See gantt-chart.png for the Gantt chart.
