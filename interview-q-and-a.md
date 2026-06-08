# Interview Q&A

## Purpose

This document prepares interview-ready answers based on the SOC 2 Access Control Audit Project.

The goal is to explain the project clearly during interviews and show practical understanding of GRC, access controls, evidence collection, risk assessment, and remediation tracking.

---

## Q1: Can you walk me through this project?

**Answer:**

This project simulates a Junior GRC Analyst assignment for a SaaS company preparing for a SOC 2 Type II audit.

The company wanted to review access management controls across systems such as Okta, Google Workspace, GitHub, AWS, HRIS, Slack, and Jira.

I created an evidence request list, performed control testing, documented findings, rated risks, created a remediation tracker, and prepared an executive summary.

The main focus was to determine whether access controls were properly approved, reviewed, removed, documented, and retained as audit-ready evidence.

---

## Q2: What controls did you review?

**Answer:**

I focused on access management controls, including:

- Quarterly user access reviews
- Terminated user access removal
- Privileged access review
- MFA enforcement
- Access request approvals
- New hire access provisioning
- Role change access updates
- Service account ownership
- Evidence retention
- Exception management

These areas are important because they help prove that users only have appropriate access and that access is removed or changed when needed.

---

## Q3: What evidence would you request for user access reviews?

**Answer:**

For user access reviews, I would request:

- User access review report
- List of users and roles
- Reviewer name and sign-off
- Date the review was completed
- Exceptions identified during the review
- Remediation evidence for removed or modified access
- System exports from tools like Okta, GitHub, AWS, or Google Workspace

The evidence should be complete, dated, approved, and stored in a centralized audit evidence folder.

---

## Q4: What was the highest-risk finding?

**Answer:**

The highest-risk finding was delayed removal of terminated user access.

In the mock testing sample, 2 out of 10 terminated users retained access for more than 5 business days after termination.

This is high risk because former employees may still access company systems, customer data, internal documentation, or source code after leaving the company.

The recommended remediation was to implement a 24-hour offboarding SLA and require HR to notify IT through a formal Jira ticket immediately after termination is entered in the HRIS.

---

## Q5: How did you rate the risks?

**Answer:**

I rated risks using likelihood and impact.

For example, delayed offboarding was rated High because the likelihood was high and the impact was high. If a terminated employee retains access, there is a direct risk of unauthorized access.

For MFA exceptions without approval, I rated the risk Medium because the impact can be serious, but the risk depends on whether compensating controls exist and whether the accounts are actively used.

The goal was to make the risk rating practical and tied to business impact.

---

## Q6: What is the difference between a control gap and a risk?

**Answer:**

A control gap is a weakness in a process or control.

A risk is the possible business impact that could happen because of that weakness.

For example, missing sign-off on an access review is the control gap. The risk is that inappropriate or excessive access may remain active without management awareness, which could lead to unauthorized access or audit exceptions.

---

## Q7: How would you explain this project to a hiring manager?

**Answer:**

I built a SOC 2-style access control audit project to demonstrate practical GRC work.

I created realistic audit deliverables, including an evidence request list, control testing worksheet, risk register, remediation tracker, findings report, and executive summary.

The project helped me practice how to collect evidence, test controls, identify gaps, rate risks, write findings, and communicate remediation priorities to leadership.

---

## Q8: What did you learn from this project?

**Answer:**

I learned that in GRC, having a control is not enough. The organization must be able to prove the control is operating effectively through complete and reliable evidence.

I also learned how important access management is for SOC 2 readiness, especially offboarding, privileged access, access reviews, MFA, and exception management.

This project helped me understand how audit findings are connected to business risk and remediation planning.

---

## Q9: How would you handle missing audit evidence?

**Answer:**

First, I would confirm whether the evidence exists in another location or system.

If it does not exist, I would document the gap clearly, explain the risk, and work with the control owner to define remediation.

For example, if an access review was performed but no sign-off was retained, I would document that evidence is incomplete and recommend updating the access review process to require reviewer name, date, sign-off, exceptions, and remediation notes.

---

## Q10: How would you follow up on remediation?

**Answer:**

I would track each finding in a remediation tracker with the finding ID, risk level, owner, corrective action, due date, status, and evidence needed for closure.

Once the owner says the issue is fixed, I would request evidence and validate whether the remediation actually addresses the finding.

If the evidence is complete, I would mark the item as closed. If not, I would keep it open or move it to pending validation.

---

## Q11: What systems did you include in scope and why?

**Answer:**

The systems in scope included Okta or Microsoft Entra ID, Google Workspace or Microsoft 365, GitHub, AWS, HRIS, Slack, and Jira.

These systems were selected because they represent common SaaS company systems where access control risk is important.

Okta is important for identity and MFA. GitHub and AWS are important because they may contain source code and production access. HRIS is important for employee lifecycle events. Jira is important because it stores access request and approval evidence.

---

## Q12: How does this project relate to SOC 2?

**Answer:**

SOC 2 focuses on whether a company has controls in place to protect customer data and operate securely.

Access controls are a major part of SOC 2 readiness because companies need to prove that users are approved, reviewed, removed when necessary, and monitored.

This project supports SOC 2 readiness by reviewing access management controls, testing evidence, identifying gaps, and tracking remediation.

---

## Q13: What would you do differently in a real company?

**Answer:**

In a real company, I would work directly with control owners, system administrators, HR, IT, and compliance teams.

I would request actual system exports, screenshots, tickets, policies, and approval records.

I would also validate evidence directly against the source systems when possible and make sure remediation actions are practical for the business.

---

## Q14: How would you explain your lack of formal GRC job experience?

**Answer:**

I would be honest and say that I am transitioning into GRC, but I have been building practical job-like projects to develop the skills required for junior GRC work.

This SOC 2 access control project allowed me to practice evidence collection, control testing, risk rating, findings documentation, remediation tracking, and executive reporting.

I understand that real company experience is different, but this project shows that I understand the workflow and can contribute with guidance.

---

## Q15: Give me a short version of the project for an interview.

**Answer:**

I built a SOC 2 access control audit simulation for a mock SaaS company. I reviewed access management controls, created an evidence request list, tested sample controls, documented findings, rated risks, built a remediation tracker, and wrote an executive summary.

The biggest risks I identified were delayed offboarding, excessive privileged access, incomplete access review sign-off, and unmanaged service accounts.

This project helped me practice realistic junior GRC analyst work from evidence collection to remediation tracking.

---

## Notes

This Q&A document is part of a mock GRC portfolio project. It is designed to help explain the project clearly in interviews and connect the deliverables to real GRC analyst responsibilities.
