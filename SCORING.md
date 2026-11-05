MK MEDIA — EVIDENCE CLASSIFICATION AND REVIEW GOVERNANCE

Challenge: MKM-GCEC-001

Document version: 1.0

Last updated: 2026-11-05

1. Purpose

This document defines how evidence-backed answers are classified and reviewed. It applies to a specific claim within a declared scope. It does not certify an organization, product, model or overall security posture.

The purpose is not to reward confident answers or punish missing evidence. It is to make the basis, boundary and limitations of each claim visible.

2. Unit of Assessment

Every classification must identify:

```text
Claim:
System or product:
Environment and configuration:
Threat model and adversary capabilities:
Assets and consequential actions:
Assessment period:
Included execution paths and populations:
Exclusions and limitations:
Acceptable-outcome criteria:
Evidence reviewed:
Reviewer and review date:
```

If the claim or scope is unclear, the administrative status is `CLARIFICATION REQUIRED`. Do not assign a security classification until the claim is assessable.

3. Classifications

DEMONSTRATED

Relevant, credible and appropriately reviewable evidence supports the specific claim within the declared scope.

The evidence must include:

- Direct tests or observations relevant to the claim.
- Relevant positive, negative and failure-path cases.
- Verification of actual outcomes, not only reported activity.
- Explicit exclusions and limitations.
- Meaningful independent observation, reproduction or review, or a clear explanation of why the available independent evidence is sufficient for the scoped claim.

`DEMONSTRATED` does not mean universally secure, permanently effective or proven against every adversary.

PARTIAL

Direct evidence supports part of the claim, but one or more material gaps remain, such as:

- Incomplete path or population coverage.
- Missing negative or failure-condition tests.
- Unverified actual outcomes.
- Material unverified dependencies.
- Limited independence or reproducibility.
- Outdated evidence for a materially changed system.

The supported boundary and remaining gap must be explicit.

UNKNOWN

Available evidence is insufficient to determine whether the claim holds. This includes evidence that is unavailable, incomplete, not yet assessable or not safely shareable.

`UNKNOWN` does not imply weakness, failure or dishonesty.

NOT DEMONSTRATED

An answer was provided, but its assertions, policies, certifications or supplied artifacts do not substantiate the specific claim.

This describes the answer’s evidentiary support. It is not a finding that the system is insecure.

FAILED

Relevant testing or credible evidence establishes that the claimed protection did not hold within the assessed scope.

`FAILED` requires evidence that contradicts the claim. Missing evidence alone must never be classified as `FAILED`.

NOT ASSESSED — Administrative Status

No assessment has been performed. This is not a security classification and must not be presented as one.

4. Evidence Assessment Dimensions

Reviewers should consider the following without turning them into a mechanical points score.

Scope Relevance

Does the evidence concern the exact claim, environment, action and threat model being assessed?

Directness

Does the evidence show enforcement and consequences, or does it merely describe intent, design, policy or organizational process?

Negative and Failure-Path Coverage

Were unauthorized actions, alternate paths, revoked authority, dependency failures and relevant exceptional cases tested where applicable?

Outcome Verification

Was the resulting system state checked using appropriate system-of-record observations, business-outcome checks or independent reconciliation?

Independence and Common-Mode Risk

Could the evidence, approval, observation or review be controlled by the same compromised component or context as the claim being assessed?

Independence is a property of the evidence path, not merely a reviewer’s job title.

Recency and Change Relevance

Is the evidence current for the version and configuration assessed? Have material changes occurred since the test?

Completeness and Conflict Handling

Are exclusions, missing records, contradictory results and unresolved UNKNOWNs disclosed rather than silently omitted?

Remediation Validation

Where issues were found, is there evidence that corrective actions were completed and the relevant claim was retested?

5. Implementation Neutrality

Participants may demonstrate equivalent protection using different architectures and methods.

A particular technology or exercise style is not universally mandatory. Examples that must not become blanket requirements include:

- A specific cloud, identity, logging or enforcement vendor.
- eBPF, a particular sandbox technology or a specific blockchain.
- Cryptographic human-approval gates for every environment.
- Unannounced, destructive or live-production adversarial exercises.
- Automatic isolation where a different authorized control can safely demonstrate the claimed outcome.

Evaluate the claimed outcome and evidence, not familiarity with a preferred implementation.

All adversarial testing requires appropriate authorization, scope and operational safety controls.

6. Evidence Safety

Public responses must not contain credentials, secrets, customer information, unnecessary personal data, confidential architecture or exploitable procedures.

Acceptable approaches include:

- Redacted test summaries.
- Synthetic or laboratory exercises.
- Scoped system-of-record observations.
- Private independent review referenced without publishing sensitive artifacts.
- Explicit UNKNOWNs where evidence cannot yet be assessed or shared.

No confidential-submission channel is currently provided. Do not send confidential material to maintainers under an assumption that such a channel exists.

A hash can support later integrity verification. It does not prove occurrence, completeness, independence or control effectiveness.

7. Roles and Authority

Participant

The participant defines the claim, supplies the response, self-classifies and declares limitations. The participant is responsible for publication authority and disclosure safety.

Maintainer

Maintainers check repository form, navigation, provenance, safety and whether review records are complete. Accepting a pull request is an editorial action, not security certification.

Evidence Reviewer

An evidence reviewer evaluates only the claims, evidence and scope explicitly assigned. The reviewer must identify their independence, method, exclusions and conflicts of interest.

No reviewer may convert a scoped result into a claim about an entire company or product.

8. Conflicts of Interest

A review record must disclose relevant conflicts, including where applicable:

- Employment, contracting or financial relationships.
- Authorship or ownership of the assessed system.
- Participation in the control, approval or evidence path being reviewed.
- Dependence on the same potentially compromised component or administrative domain.
- Any incentive that could materially affect the classification.

A conflict does not automatically invalidate evidence, but it must be visible and considered when evaluating independence.

9. Review Workflow

```text
SUBMITTED
  → FORM AND SAFETY REVIEW
  → CLARIFICATION REQUIRED, if necessary
  → EVIDENCE REVIEW
  → PARTICIPANT REPLY, if requested
  → REVIEW RECORD PUBLISHED
  → CORRECTION OR APPEAL, if raised
  → CLOSED WITH VERSIONED HISTORY
```

Possible review outcomes include `DEMONSTRATED`, `PARTIAL`, `UNKNOWN`, `NOT DEMONSTRATED`, `FAILED`, `CLARIFICATION REQUIRED` and `HOLD`.

`HOLD` is appropriate for unresolved provenance, conflicting metadata, unsafe disclosure or evidence that cannot yet be handled appropriately.

10. Participant Reply and Appeal

Participants may:

- Correct factual or provenance errors.
- Clarify scope or exclusions.
- Provide additional sanitized evidence.
- Challenge a reviewer’s conflict of interest or classification rationale.
- Request correction of public presentation that overstates the review.

Use a linked issue and reference the original response and review record. Corrections must be dated and versioned. Original model submissions remain verbatim; participant responses and review records retain their correction history.

An appeal is a request for evidence-based reconsideration, not a guarantee of reclassification.

11. Review Record Template

```text
REVIEW ID:
RESPONSE AND VERSION:
CLAIM AND SCOPE:
REVIEW DATE:
REVIEWER:
REVIEWER ROLE AND INDEPENDENCE:
CONFLICTS OF INTEREST:
EVIDENCE REVIEWED:
METHOD:
POSITIVE / NEGATIVE / FAILURE-PATH COVERAGE:
OUTCOME VERIFICATION:
COMMON-MODE DEPENDENCIES:
EXCLUSIONS AND UNKNOWNS:
CLASSIFICATION:
RATIONALE:
PARTICIPANT REPLY:
CORRECTIONS OR APPEAL HISTORY:
NEXT REVIEW OR RETEST:
```

12. Claims the Repository Does Not Make

Accepting or reviewing an answer does not mean that:

- The repository maintainers certify the participant’s security.
- The entire product or organization is secure.
- A result applies outside its declared scope.
- An AI model or provider endorses the challenge or a participant.
- AI agreement constitutes independent validation.
- A certification, hash, log or dashboard is sufficient evidence by itself.
- Missing evidence proves failure.

SECURITY CLAIM ≠ SECURITY EVIDENCE

MISSING EVIDENCE ≠ PROVEN FAILURE

SCOPED DEMONSTRATION ≠ UNIVERSAL SECURITY