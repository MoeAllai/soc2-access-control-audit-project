# Executive Summary

## SOC 2 Access Control Readiness Review

## Overview

CloudCore Analytics is preparing for a SOC 2 Type II audit and requested a review of access management controls across key systems including Okta, Google Workspace, GitHub, AWS, Slack, HRIS, and Jira.

The review focused on whether access controls were properly documented, approved, reviewed, and retained as audit-ready evidence.

## Scope

The review covered the following access control areas:

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

## Overall Assessment

CloudCore Analytics has several access management controls in place, but the control environment is not yet fully audit-ready.

The main issue is not the complete absence of controls. The main issue is inconsistent evidence, missing approvals, delayed offboarding, and incomplete documentation across high-risk systems.

These gaps may create SOC 2 audit exceptions if not remediated before the audit period.

## Key Findings

| Priority | Finding | Risk Level | Business Impact |
|---|---|---|---|
| 1 | Delayed removal of terminated user access | High | Former employees may retain access to company systems after termination |
| 2 | Admin accounts without business justification | High | Excessive privileged access may increase risk of unauthorized changes or data exposure |
| 3 | Missing sign-off for GitHub and AWS access reviews | High | Company may not be able to prove access was reviewed for critical systems |
| 4 | Service accounts missing owners | High | Unowned accounts may not be monitored, reviewed, or removed when no longer needed |
| 5 | Employees retaining access after role changes | High | Users may keep access that no longer matches job responsibilities |
| 6 | MFA exceptions without approval | Medium | Authentication controls may be weakened without formal approval |
| 7 | Missing access approval evidence | Medium | Access may be granted without proof of proper authorization |
| 8 | Inconsistent evidence naming and retention | Medium | Audit evidence may be difficult to locate, validate, or rely on |

## Risk Summary

| Risk Level | Count |
|---|---|
| High | 5 |
| Medium | 5 |
| Low | 0 |

The highest-risk areas relate to unauthorized access, especially delayed offboarding, privileged access, unmanaged service accounts, and incomplete access reviews for critical systems.

## Recommended Remediation Priorities

Management should prioritize remediation in the following order:

1. Implement a 24-hour offboarding SLA for terminated users
2. Review and remove unnecessary privileged access
3. Require documented sign-off for all quarterly access reviews
4. Assign owners to all service accounts
5. Create a formal mover process for role changes
6. Document and approve all MFA/access exceptions
7. Enforce manager approval before access is granted
8. Standardize SOC 2 evidence storage and naming

## Recommended Target Timeline

| Timeline | Recommended Action |
|---|---|
| 0–15 days | Fix delayed offboarding process and require HR-to-IT termination tickets |
| 0–30 days | Review privileged access, assign service account owners, document MFA exceptions |
| 30–45 days | Improve Jira approval workflow and role change process |
| 45–60 days | Standardize evidence retention and perform validation testing |

## Business Impact

If these issues are not remediated, CloudCore Analytics may face:

- SOC 2 audit exceptions
- Increased risk of unauthorized access
- Poor evidence quality during audit review
- Excessive or inappropriate user access
- Difficulty proving control operation over time
- Higher risk from privileged and service accounts

## Analyst Conclusion

CloudCore Analytics is partially ready for a SOC 2 access control review, but remediation is needed before the company can confidently enter the Type II audit period.

The most urgent focus should be on terminated user access removal, privileged access governance, access review sign-off, and service account ownership.

Once remediation is completed, management should perform validation testing to confirm that corrective actions are operating effectively and that evidence is complete, dated, approved, and stored in the correct location.

## Project Note

This executive summary is part of a mock GRC portfolio project. It demonstrates executive reporting, risk communication, SOC 2 audit readiness, access control review, and remediation prioritization.
