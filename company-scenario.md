# Company Scenario

## Mock Company Profile

**Company Name:** CloudCore Analytics  
**Industry:** SaaS / Data Analytics  
**Company Size:** 120 employees  
**Environment:** Cloud-based SaaS platform  
**Audit Goal:** SOC 2 Type II readiness  
**Mock Role:** Junior GRC Analyst  

CloudCore Analytics is a mock SaaS company that provides analytics dashboards to small and mid-sized businesses. The company stores customer business data, user account information, internal documentation, and source code across several cloud and business systems.

The company is preparing for a SOC 2 Type II audit and wants to confirm that access management controls are properly designed, documented, and operating effectively.

## Systems in Scope

The following systems are included in the access control review:

| System | Purpose | Risk Area |
|---|---|---|
| Okta / Microsoft Entra ID | Identity provider and single sign-on | User access, MFA, privileged access |
| Google Workspace / Microsoft 365 | Email, documents, collaboration | Sensitive internal data access |
| GitHub | Source code repository | Code access, admin permissions |
| AWS | Cloud infrastructure | Production access, privileged roles |
| Slack | Internal communication | Internal information exposure |
| HRIS System | Employee lifecycle management | Joiner, mover, leaver process |
| Jira | Ticketing and workflow tracking | Access request and approval evidence |

## Business Problem

CloudCore Analytics has grown quickly from 40 employees to 120 employees. Access management processes were informal in the past, but the company now needs stronger governance because of SOC 2 audit requirements.

Management is concerned that:

- User access reviews may not be performed consistently
- Terminated employees may retain access after leaving the company
- Privileged access may not be properly reviewed
- MFA enforcement may not be fully documented
- Audit evidence may be missing or incomplete
- Vendor risk documentation may not be centralized

## Assignment

As a Junior GRC Analyst, the task is to support SOC 2 audit readiness by reviewing access management controls, collecting evidence, identifying control gaps, rating risks, and documenting remediation actions.

## Scope of Review

This project focuses on the following areas:

1. User access review process  
2. Terminated user access removal  
3. Privileged account review  
4. MFA enforcement  
5. Access request approval evidence  
6. Evidence retention  
7. Remediation tracking  

## Key Control Objectives

| Control Area | Objective |
|---|---|
| Access Reviews | Confirm user access is reviewed on a regular basis |
| Offboarding | Confirm terminated users are removed from systems timely |
| MFA | Confirm MFA is enforced for users, especially privileged users |
| Privileged Access | Confirm admin access is limited and approved |
| Access Requests | Confirm new access is approved before being granted |
| Evidence Retention | Confirm audit evidence is stored and available |
| Remediation | Confirm identified gaps are tracked to closure |

## Mock Manager Request

Mohammed,

We are preparing for our SOC 2 Type II audit and need support reviewing our access management controls. Please help us identify what evidence we need, test a sample of access controls, document any gaps, and prepare a remediation tracker for leadership review.

Please focus on user access reviews, offboarding, MFA, privileged access, and evidence quality.

Expected deliverables:

- Evidence request list
- Control testing worksheet
- Risk register updates
- Findings summary
- Remediation tracker
- Executive summary

Thanks,  
GRC Manager

## Assumptions

This is a mock GRC portfolio project created for learning and demonstration purposes. No real company data, employee data, vendor data, or confidential information is used.

The project is designed to simulate realistic junior GRC analyst work related to SOC 2 audit readiness, access control testing, evidence collection, risk assessment, and remediation tracking.
