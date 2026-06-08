# Control Testing Worksheet

## Purpose

This worksheet documents sample control testing performed for CloudCore Analytics as part of SOC 2 Type II readiness.

The goal is to determine whether access management controls are designed properly and operating effectively.

## Control Testing Table

| Test ID | Control ID | Control Description | Test Procedure | Sample Reviewed | Test Result | Status | Notes / Finding |
|---|---|---|---|---|---|---|---|
| T-01 | AC-01 | User access reviews are performed quarterly for in-scope systems | Reviewed latest quarterly access review report for Okta, GitHub, AWS, and Google Workspace. Checked for reviewer, completion date, user list, exceptions, and sign-off. | Q1 access review package | Access review completed for Okta and Google Workspace, but GitHub and AWS reviews were missing reviewer sign-off. | Partial Pass | Evidence incomplete for privileged systems |
| T-02 | AC-02 | Terminated users are removed from systems within 24 hours of termination | Compared HR termination report against Okta deactivation logs and Jira offboarding tickets. | 10 terminated users | 8 users were removed within 24 hours. 2 users were removed after 5+ business days. | Fail | Delayed offboarding creates unauthorized access risk |
| T-03 | AC-03 | Privileged access is reviewed quarterly by management | Reviewed admin user exports from Okta, AWS, and GitHub and checked for management approval. | 15 admin accounts | 3 admin accounts had no documented business justification. | Fail | Excessive privileged access identified |
| T-04 | AC-04 | MFA is enforced for all users and administrators | Reviewed MFA policy screenshot and enrolled user report from Okta. | All active users | MFA enabled for 117 of 120 users. 3 service accounts excluded without documented approval. | Partial Pass | MFA exceptions need approval and expiration date |
| T-05 | AC-05 | Access requests are approved before access is granted | Reviewed Jira tickets for new access requests and compared approval time against access grant time. | 20 access request tickets | 18 tickets had proper approval before access was granted. 2 tickets had missing approval evidence. | Partial Pass | Approval evidence not consistently retained |
| T-06 | AC-06 | New hire access is provisioned based on job role | Compared HR new hire records, approved role, and access granted in Okta. | 10 new hires | 9 users received access aligned to job role. 1 user received access to an unnecessary GitHub group. | Partial Pass | Role-based access needs review |
| T-07 | AC-07 | Role changes trigger access updates | Reviewed employee transfer records and access change tickets. | 5 role changes | 2 employees retained access from previous roles. | Fail | Mover process is not consistently followed |
| T-08 | AC-08 | Shared and service accounts are approved and monitored | Reviewed service account inventory and owner approval records. | 8 service accounts | 5 accounts had owners and justification. 3 accounts had no documented owner. | Fail | Service account ownership missing |
| T-09 | AC-09 | Audit evidence is retained in a centralized location | Reviewed evidence folder structure and naming convention. | SOC 2 evidence folder | Evidence exists but naming is inconsistent and some files are missing dates. | Partial Pass | Evidence retention process needs standardization |
| T-10 | AC-10 | Access control exceptions are documented, approved, and time-bound | Reviewed exception register for MFA and privileged access exceptions. | 6 exceptions | 4 exceptions had approval and expiration dates. 2 were open-ended. | Partial Pass | Exceptions should not be permanent without review |

## Testing Summary

| Result | Count |
|---|---|
| Pass | 0 |
| Partial Pass | 6 |
| Fail | 4 |
| Total Tests | 10 |

## Key Observations

The access control environment is partially mature, but several issues require remediation before the SOC 2 audit.

Main issues identified:

- Incomplete access review evidence for GitHub and AWS
- Delayed offboarding for terminated users
- Missing business justification for privileged accounts
- MFA exceptions without documented approval
- Access approvals not consistently retained
- Role change access not consistently updated
- Service accounts missing owners
- Evidence files not consistently named or dated

## Analyst Conclusion

Based on the testing performed, CloudCore Analytics has access control processes in place, but evidence quality and consistency need improvement.

The highest risk areas are terminated user access removal, privileged access review, and service account ownership. These areas should be prioritized for remediation before the SOC 2 Type II audit period.

## Recommended Next Steps

1. Enforce quarterly access reviews for all in-scope systems
2. Require documented sign-off for each access review
3. Implement a 24-hour offboarding SLA
4. Review and remove unnecessary privileged access
5. Document all MFA exceptions with approval and expiration dates
6. Assign owners to all service accounts
7. Standardize audit evidence naming and storage
8. Track all findings in a remediation tracker

## Notes

This control testing worksheet is part of a mock GRC portfolio project. It demonstrates control testing, evidence review, audit readiness, risk identification, and remediation planning skills.
