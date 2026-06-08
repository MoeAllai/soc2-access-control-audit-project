# Remediation Tracker

## Purpose

This remediation tracker documents corrective actions for access control gaps identified during the SOC 2 readiness review for CloudCore Analytics.

The goal is to track each finding from identification through remediation, assign ownership, define due dates, and monitor progress until closure.

## Remediation Tracker Table

| Finding ID | Related Risk | Finding Title | Risk Level | Corrective Action | Owner | Target Due Date | Status | Evidence Needed for Closure |
|---|---|---|---|---|---|---|---|---|
| F-01 | R-01 | Missing Sign-Off for GitHub and AWS Access Reviews | High | Require documented reviewer sign-off for all quarterly access reviews, including GitHub and AWS. Update access review template to include reviewer name, date, exceptions, and approval. | IT Manager | 30 days | Open | Completed GitHub and AWS access review reports with reviewer sign-off |
| F-02 | R-02 | Delayed Removal of Terminated User Access | High | Implement a 24-hour offboarding SLA. Require HR to notify IT immediately through Jira when an employee termination is entered in the HRIS. | HR + IT | 15 days | Open | HR termination report, Jira offboarding tickets, Okta deactivation logs |
| F-03 | R-03 | Admin Accounts Without Business Justification | High | Review all privileged accounts and remove unnecessary admin access. Require business justification and approval for retained admin accounts. | IT Security | 30 days | Open | Updated admin user list, approval records, justification notes |
| F-04 | R-04 | MFA Exceptions Without Approval | Medium | Create an MFA exception register requiring owner, approval, business justification, compensating control, and expiration date. | IT Security | 30 days | Open | MFA exception register with approvals and expiration dates |
| F-05 | R-05 | Missing Access Approval Evidence | Medium | Update Jira workflow to require manager approval before access provisioning tickets can be closed. | IT Helpdesk | 45 days | Open | Jira ticket samples showing approval before access grant |
| F-06 | R-06 | New Hire Received Unnecessary GitHub Access | Medium | Review role-based access templates and remove unnecessary access from default new hire profiles. | HR + IT | 30 days | Open | Updated role-based access matrix and corrected user access record |
| F-07 | R-07 | Employees Retained Access After Role Change | High | Create a mover access review workflow for internal transfers. Require removal of old role access and approval of new role access. | HR + IT | 45 days | Open | Role change tickets, removed access evidence, new approval records |
| F-08 | R-08 | Service Accounts Missing Owners | High | Assign a business owner to every service account and require quarterly review of service account access. | IT Security | 30 days | Open | Service account inventory with owner, purpose, and review date |
| F-09 | R-09 | Inconsistent Evidence Naming and Retention | Medium | Standardize SOC 2 evidence folder structure, file naming convention, ownership, and retention requirements. | Compliance | 45 days | Open | Updated evidence folder, naming standard, retention procedure |
| F-10 | R-10 | Open-Ended Access Exceptions | Medium | Require all access control exceptions to include approval, expiration date, compensating control, and periodic review. | Compliance + IT Security | 30 days | Open | Exception register showing approval, expiration, and review schedule |

## Status Definitions

| Status | Meaning |
|---|---|
| Open | Finding has been identified but remediation has not started |
| In Progress | Corrective action is actively being worked on |
| Pending Validation | Remediation is complete and awaiting evidence review |
| Closed | Evidence has been reviewed and remediation is complete |
| Risk Accepted | Management formally accepted the risk |

## Remediation Priority

The highest priority items are:

1. Delayed terminated user access removal
2. Privileged accounts without business justification
3. Missing sign-off for GitHub and AWS access reviews
4. Service accounts without owners
5. Employees retaining access after role changes

## Analyst Notes

The remediation plan focuses first on high-risk access control issues that could lead to unauthorized access or SOC 2 audit exceptions.

The most urgent remediation item is delayed offboarding because terminated users retaining access creates a direct security and compliance risk.

Privileged access and service account ownership should also be prioritized because these accounts often have elevated permissions and may create greater impact if misused.

## Executive Summary

The SOC 2 access control review identified several gaps related to access review evidence, offboarding, privileged access, MFA exceptions, service account ownership, and evidence retention.

Corrective actions have been assigned to IT, HR, IT Security, Helpdesk, and Compliance teams. High-risk findings should be remediated within 15 to 30 days, while medium-risk findings should be completed within 30 to 45 days.

Successful closure requires documented evidence, including system exports, approval records, Jira tickets, access review reports, exception registers, and updated procedures.

## Notes

This remediation tracker is part of a mock GRC portfolio project. It demonstrates remediation planning, issue tracking, ownership assignment, audit readiness, and risk management skills.
