# Findings Report

## Purpose

This findings report summarizes access control gaps identified during the SOC 2 readiness review for CloudCore Analytics.

The goal is to document each issue in a clear audit-style format, including business impact, root cause, risk level, and recommended remediation.

## Finding 1: Missing Sign-Off for GitHub and AWS Access Reviews

**Risk Level:** High  
**Related Control:** AC-01  
**Related Risk:** R-01  
**Owner:** IT Manager  

### Observation

The quarterly access review package included evidence for Okta and Google Workspace, but GitHub and AWS access reviews were missing documented reviewer sign-off.

### Business Impact

Without reviewer sign-off, the company cannot prove that access to high-risk systems was reviewed and approved. This may create SOC 2 audit exceptions and increase the risk of unauthorized access remaining undetected.

### Root Cause

The access review process was not consistently applied across all in-scope systems.

### Recommendation

Require documented reviewer sign-off for every quarterly access review, including reviewer name, completion date, exceptions identified, and remediation actions.

---

## Finding 2: Delayed Removal of Terminated User Access

**Risk Level:** High  
**Related Control:** AC-02  
**Related Risk:** R-02  
**Owner:** HR + IT  

### Observation

Out of 10 terminated users reviewed, 2 users retained system access for more than 5 business days after termination.

### Business Impact

Delayed offboarding may allow former employees to access company systems, customer data, internal documentation, or source code after employment ends.

### Root Cause

The termination notification process between HR and IT is not consistently tracked through a formal ticketing workflow.

### Recommendation

Implement a 24-hour offboarding SLA and require HR to submit termination tickets to IT immediately when termination is entered in the HRIS.

---

## Finding 3: Admin Accounts Without Business Justification

**Risk Level:** High  
**Related Control:** AC-03  
**Related Risk:** R-03  
**Owner:** IT Security  

### Observation

Three admin accounts had no documented business justification or approval record.

### Business Impact

Unnecessary privileged access increases the risk of unauthorized changes, data exposure, system misuse, and audit findings.

### Root Cause

Privileged access was granted historically but not reviewed against current job responsibilities.

### Recommendation

Review all admin accounts, remove unnecessary privileges, and require documented business justification for any retained administrative access.

---

## Finding 4: MFA Exceptions Without Approval

**Risk Level:** Medium  
**Related Control:** AC-04  
**Related Risk:** R-04  
**Owner:** IT Security  

### Observation

Three service accounts were excluded from MFA without documented approval, expiration date, or compensating control.

### Business Impact

Unapproved MFA exceptions weaken authentication controls and may increase the risk of account compromise.

### Root Cause

The company does not maintain a formal exception register for MFA exclusions.

### Recommendation

Create an MFA exception register that includes owner, approval, business justification, compensating control, review date, and expiration date.

---

## Finding 5: Missing Access Approval Evidence

**Risk Level:** Medium  
**Related Control:** AC-05  
**Related Risk:** R-05  
**Owner:** IT Helpdesk  

### Observation

Two access request tickets did not include documented manager approval before access was granted.

### Business Impact

Access may be granted without proper authorization, increasing the risk of excessive or inappropriate access.

### Root Cause

The Jira workflow does not require approval evidence before ticket closure.

### Recommendation

Update the Jira workflow to require manager approval before access provisioning tickets can be completed.

---

## Overall Conclusion

CloudCore Analytics has access management controls in place, but the controls are not consistently documented, reviewed, or retained as audit-ready evidence.

The highest-risk findings relate to terminated user access, privileged access, and missing access review sign-off for critical systems.

Before the SOC 2 Type II audit period begins, management should prioritize remediation of high-risk findings and improve evidence consistency across all in-scope systems.

## Notes

This findings report is part of a mock GRC portfolio project. It demonstrates audit finding documentation, root cause analysis, business impact writing, risk rating, and remediation planning.
