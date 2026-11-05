MK MEDIA — GLOBAL CYBERSECURITY EVIDENCE CHALLENGE

Public Answer and Evidence Template

Prompt ID: MKM-GCEC-001

Template version: 1.0

Use one copy of this template for each specific claim. Answer one challenge question or all five. A narrow, well-supported answer is more valuable than a broad assurance without evidence.

> Do not submit credentials, secrets, customer information, confidential architecture or exploitable procedures. Use redacted artifacts, synthetic environments, scoped summaries or private independent verification. An honest `UNKNOWN` is welcome.

---

A. Response Metadata

```text
RESPONSE TITLE:
RESPONSE DATE AND TIME (WITH TIME ZONE):
PARTICIPANT / ORGANIZATION: [Public name / anonymized identifier]
RESPONDENT ROLE:
PUBLIC CONTACT OR RESPONSE LINK: [Optional]
CHALLENGE QUESTION: [1 Authority / 2 Bypass / 3 Compromised Trust / 4 Consequence / 5 Recovery Truth]
SYSTEM OR PRODUCT ASSESSED: [Public-safe identifier]
ASSESSMENT TYPE: [Conceptual review / laboratory test / production exercise / real incident / independent assessment / other]
RESPONSE VISIBILITY: [Public / private evidence available for controlled review]
SELF-ASSESSMENT: [DEMONSTRATED / PARTIAL / UNKNOWN / NOT DEMONSTRATED / FAILED]
```

The self-assessment applies only to the claim and scope declared below—not to the entire product or organization.

---

B. Short Public Answer

Maximum: 200 words.

State the claim, what was tested, what happened, what evidence supports the answer and what remains unknown.

```text
[Write the short public answer here.]
```

One-Sentence Bottom Line

```text
[Example structure: Within [scope], [specific claim] is [classification] based on [evidence type], with [material limitation] remaining.]
```

---

C. Claim and Scope

C1. Exact Claim Being Assessed

```text
[State one falsifiable claim. Avoid “we are secure” or similarly unbounded claims.]
```

C2. System and Environment Boundary

```text
System components included:
Environment: [Production / staging / laboratory / synthetic / mixed]
Relevant user, service or AI-agent populations:
Relevant interfaces and execution paths:
Assessment period:
Version or configuration assessed:
```

C3. Assets and Outcomes That Matter

```text
Assets or operations requiring protection:
Security-sensitive actions:
Criteria for an acceptable outcome:
Potential business, customer or safety consequences:
```

C4. Threat Model

```text
Adversaries or failure sources considered:
Trusted components that could fail:
Human, automated and AI-agent actions considered:
Attacker capabilities assumed:
Risks knowingly accepted:
```

C5. Exclusions and Limitations

```text
Components, paths, populations or scenarios not assessed:
Evidence not available:
Evidence that cannot be publicly disclosed:
Known assumptions and dependencies:
Remaining UNKNOWNs:
```

---

D. Test and Assessment Method

D1. Method

```text
Test or assessment method:
Test date and duration:
Test environment:
Test authorization and safety controls:
Roles involved:
Whether the exercise was announced:
Why the method was appropriate for the claim:
```

An unannounced or live-environment exercise is not universally required. Use a method proportionate to the claim, operational risk and available authorization.

D2. Test Matrix

Include relevant positive, negative, alternate-path and failure-condition tests.

Case ID	Actor / identity	Action and resource	Path / condition	Expected result	Observed result	Outcome verified?	Evidence reference	
T-01								
T-02								
T-03								

D3. Actual Outcome Verification

```text
How the resulting system state was checked:
System-of-record or independent observations used:
Expected versus observed outcome:
Unauthorized side effects checked:
Missing or conflicting evidence:
How partial completion, retries or misleading success responses were handled:
```

A successful API response, closed ticket, alert or log entry alone does not establish the final outcome.

---

E. Question-Specific Evidence

Complete the module for the question being answered. Delete unused modules in a public response if desired.

E1. The Authority Test

```text
Identity, action, resource and context evaluated:
Delegation chain and originating caller:
Effective policy or authorization version:
Enforcement point:
Missing, expired, excessive or revoked-authority tests:
Administrative, service-to-service, worker, retry and direct-API paths tested:
Behavior when authorization dependencies fail or return malformed responses:
Revocation test and subsequent-action result:
Coverage limits:
```

E2. The Bypass Test

```text
Declared enforcement boundary:
Relevant execution-path inventory:
Alternative, legacy, emergency, background and privileged paths tested:
Resource-side enforcement evidence:
How unmediated paths would be detected:
Independent review of coverage assumptions:
Excluded or unknown paths:
```

E3. The Compromised Trust Test

```text
Trusted component or workflow assumed compromised:
Potential blast radius:
Controls independent of the compromised component:
Common-mode dependencies:
Detection and containment method:
Revocation, credential rotation or update-containment results:
Clean recovery method:
Exercise date, scope and result:
Residual exposure:
```

E4. The Consequence Test

Reconstruct the complete chain.

```text
Requested action:
User or authorized intent:
Applicable authorization and policy context:
Enforcement decision:
Actual operation and system consequence:
Final business or security outcome:
Acceptability criteria:
Independent reconciliation performed:
Missing, conflicting or incomplete records:
Difference between reported success and verified outcome:
```

E5. The Recovery Truth Test

```text
Failure or compromise scenario:
Detection, escalation and containment timeline:
Named response decision authority:
Evidence sources independent of compromised domains:
Clean recovery-point selection:
Identity and credential recovery:
Declared recovery objectives:
Measured recovery results:
Data-integrity and representative business-transaction checks:
Persistence checks:
Restored security conditions independently verified:
Missed objectives and residual risks:
```

A restarted or available service is not automatically a trustworthy recovered service.

---

F. Independent Observation or Verification

Complete if applicable; otherwise write `UNKNOWN` or `NONE`.

```text
Reviewer, observer or reproducer:
Relationship to the team or vendor:
Independence from the claim and control being assessed:
Review date:
Method and scope:
Evidence inspected:
Tests independently repeated:
Outcome:
Exclusions and limitations:
Private review arrangements, if applicable:
```

Independence is a property of the evidence path, not merely a job title. An approval or observation controlled by the same potentially compromised context should be identified as a common-mode dependency.

---

G. Findings, Failures and Corrective Actions

G1. What Worked

```text
[Describe only what the evidence supports.]
```

G2. What Failed, Was Missed or Took Longer Than Expected

```text
[Include failures, near misses, attempted bypasses and unexpected outcomes.]
```

G3. Corrective-Action Register

Action ID	Finding	Corrective action	Accountable owner	Due date	Status	Retest / validation evidence	
CA-01							

No sensitive personal information is required. Use role identifiers where appropriate.

---

H. Evidence Register

List the artifacts supporting the answer. Public links are optional; controlled private evidence may be identified without disclosing its contents.

Evidence ID	Artifact or observation	Date	Source / custodian	Public or private	Redaction status	Integrity reference (optional)	Scope and limitations	
E-01								
E-02								

An integrity hash can support later integrity verification; it does not prove that an event occurred, that evidence is complete or that a control is effective.

---

I. Classification and Rationale

Select one classification for the specific claim and scope.

```text
[ ] DEMONSTRATED
    Relevant, credible and reviewable evidence supports the claim within the declared scope. Actual outcomes and relevant negative or failure paths have been checked.

[ ] PARTIAL
    Evidence supports part of the claim, but material coverage, independence, recency, dependency or outcome-verification gaps remain.

[ ] UNKNOWN
    Evidence is insufficient to determine whether the claim holds. This does not imply weakness or failure.

[ ] NOT DEMONSTRATED
    The answer or supplied artifacts do not substantiate the claim. This does not establish that the system is insecure.

[ ] FAILED
    Relevant testing or credible evidence establishes that the claimed protection did not hold within the assessed scope. Do not select FAILED merely because evidence is missing.
```

```text
Classification selected:
Evidence supporting the classification:
Material limitations:
Why a higher classification is not currently justified:
Claims explicitly not being made:
```

---

J. Publication Safety Checklist

Confirm each item before public submission.

```text
[ ] No credentials, secrets, access tokens or private keys are included.
[ ] No customer or unnecessary personal information is included.
[ ] No confidential architecture or exploitable procedures are exposed.
[ ] Redactions have been reviewed.
[ ] Public claims match the evidence and declared scope.
[ ] Limitations and UNKNOWNs are visible.
[ ] Independent-review claims accurately represent the reviewer’s role and scope.
[ ] The respondent has authority to publish this response.
[ ] Sensitive supporting evidence has an appropriate controlled-review path, if offered.
```

---

K. Participant Declaration

```text
This response addresses only the claim and scope declared above. It does not claim that the entire system, product or organization is secure. The response distinguishes observed evidence from assumptions and identifies material limitations and UNKNOWNs.

RESPONDENT:
ROLE:
DATE:
DECLARATION: [Confirmed / Not confirmed]
```

Final Reminder

SECURITY CLAIM ≠ SECURITY EVIDENCE

AUTHENTICATION ≠ AUTHORIZATION

CORRECT DECISION ≠ COMPLETE ENFORCEMENT

LOGGED EVENT ≠ VERIFIED CONSEQUENCE

SUCCESSFUL EXECUTION ≠ ACCEPTABLE OUTCOME

RESTORED SERVICE ≠ RESTORED SECURITY

An honest `UNKNOWN` is better than an invented `PASS`.