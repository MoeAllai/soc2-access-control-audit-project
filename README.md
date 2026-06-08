# SOC 2 Access Control Audit Project

## Project Overview

This project simulates a Junior GRC Analyst assignment for a mock SaaS company preparing for a SOC 2 Type II audit.

The goal of this project is to demonstrate practical GRC skills in access control review, audit evidence collection, control testing, risk assessment, findings documentation, remediation tracking, and executive reporting.

## Mock Scenario

CloudCore Analytics is a 120-employee SaaS company that provides analytics dashboards to business customers. The company is preparing for a SOC 2 Type II audit and needs to validate whether access management controls are properly designed, documented, and operating effectively.

The review focuses on systems commonly used in SaaS environments, including identity management, cloud infrastructure, source code repositories, collaboration tools, ticketing systems, and HR systems.

## Project Scope

The review covers the following access control areas:

- User access reviews
- Terminated user access removal
- Privileged access review
- MFA enforcement
- Access request approvals
- New hire access provisioning
- Role change access updates
- Shared and service account ownership
- Evidence retention
- Exception management
- Remediation tracking

## Key Deliverables

| Deliverable | Description |
|---|---|
| [Company Scenario](company-scenario.md) | Mock company background, audit scope, systems in scope, and manager request |
| [Evidence Request List](evidence-request-list.md) | Audit evidence needed to test access management controls |
| [Control Testing Worksheet](control-testing-worksheet.md) | Sample testing procedures, results, observations, and control gaps |
| [Risk Register](risk-register.md) | Business risks identified from control testing results |
| [Remediation Tracker](remediation-tracker.md) | Corrective action plan with owners, due dates, statuses, and closure evidence |
| [Findings Report](findings-report.md) | Audit-style findings with business impact, root cause, and recommendations |
| [Executive Summary](executive-summary.md) | Leadership-level summary of risks, findings, and remediation priorities |
| [Interview Q&A](interview-q-and-a.md) | Interview-ready answers explaining the project and GRC workflow |
| [References](references.md) | Frameworks, concepts, simulated tools, and project disclaimer |

## Skills Demonstrated

- GRC analysis
- SOC 2 audit readiness
- Access control testing
- Evidence collection and review
- Risk identification and rating
- Audit finding documentation
- Root cause analysis
- Remediation tracking
- Executive reporting
- Identity and access management concepts
- Privileged access governance
- Offboarding control review
- Exception management
- Service account ownership review

## Systems Simulated

| System | Purpose |
|---|---|
| Okta / Microsoft Entra ID | Identity provider, MFA, user access reports |
| Google Workspace / Microsoft 365 | Email, documents, and collaboration access |
| GitHub | Source code repository and admin permissions |
| AWS | Cloud infrastructure and privileged access |
| Jira | Access request tickets and approval evidence |
| HRIS | Employee lifecycle records |
| Slack | Internal communication system |

## Key Findings Summary

The review identified several access control gaps, including:

- Delayed removal of terminated user access
- Admin accounts without business justification
- Missing sign-off for GitHub and AWS access reviews
- Service accounts without documented owners
- Employees retaining access after role changes
- MFA exceptions without approval or expiration dates
- Missing access approval evidence
- Inconsistent evidence naming and retention

## Analyst Conclusion

CloudCore Analytics has access management controls in place, but the control environment is not fully audit-ready.

The highest-priority remediation items are terminated user access removal, privileged access governance, access review sign-off, service account ownership, and role-change access updates.

This project demonstrates how a Junior GRC Analyst can support SOC 2 readiness by collecting evidence, testing controls, documenting findings, rating risks, and tracking remediation to closure.

## Project Disclaimer

This is a mock GRC portfolio project created for educational and demonstration purposes.

All company names, systems, findings, evidence, risks, and remediation actions are fictional. No real company data, employee data, customer data, credentials, audit evidence, or confidential information is used.
