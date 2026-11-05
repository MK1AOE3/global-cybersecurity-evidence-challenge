# MK MEDIA — THE GLOBAL CYBERSECURITY EVIDENCE CHALLENGE

**Prompt ID:** MKM-GCEC-001  
**Challenge version:** 1.0  
**README revision:** 1.1  
**Last updated:** 2026-11-05  
**Status:** Open, vendor-neutral conceptual research challenge  
**Initiated by:** Musab / MK MEDIA

## The One Question Behind All Five

> **Why should we trust your model—and what independently verifiable evidence shows that this trust is justified?**

For a security product, automated system or organization, the same challenge becomes:

> **Why should we trust your security claim—and what evidence survives independent scrutiny?**

Not confidence. Not reputation. Not popularity. Not a polished demonstration. Not a compliance badge. Evidence.

Trust must be scoped: trusted for which decision, under whose authority, in which environment, against which threats, and with what consequences when the model or system is wrong?

## Start Here

| I want to… | Go to |
|---|---|
| Answer the challenge | [Answer Template](ANSWER_TEMPLATE.md) |
| Understand how to submit a public answer | [Public Response Guide](responses/README.md) |
| Read the unchanged master prompt | [PROMPT.md](PROMPT.md) |
| Understand classifications and review governance | [SCORING.md](SCORING.md) |
| Read the model submissions | [Submission Index](submissions/README.md) |
| Read the cross-model reviewer analysis | [Model Comparison](reviews/model-comparison.md) |
| Check unresolved attribution | [Provenance HOLD Register](reviews/provenance-hold.md) |
| See document history | [CHANGELOG.md](CHANGELOG.md) |

### Quick Participation

1. Choose one of the [five evidence challenges](#the-five-evidence-challenges).
2. Copy [ANSWER_TEMPLATE.md](ANSWER_TEMPLATE.md) and answer one specific, scoped claim.
3. Follow the [Public Response Guide](responses/README.md) and submit your answer through a pull request under `responses/`.
4. Use an issue for questions, provenance corrections or a review-related reply.
5. Do not submit secrets, customer information, confidential architecture or exploitable procedures.

A confidential-submission channel is **not currently provided**. Private evidence may be referenced without posting it, but no confidential upload service is promised by this repository.

## Why This Challenge Exists

Cybersecurity language is easy to produce. Demonstrated protection is harder.

A system can have strong authentication and still permit an unauthorized action. A security control can make the correct decision and still be bypassed. A trusted component can become the attack path. A dashboard can report success while the real-world outcome is unacceptable. A service can restart after an incident without its security being restored.

This challenge invites cybersecurity companies, AI developers, researchers, CISOs, security architects, engineers and security professionals to replace broad assurances with scoped, credible and appropriately verifiable evidence.

The objective is collective improvement—not public embarrassment.

## What This Repository Contains

- The [unchanged master prompt](PROMPT.md) used to ask multiple AI models for their strongest five security questions.
- Separate [Markdown submissions](submissions/README.md) preserving each accepted model response.
- A public [answer template](ANSWER_TEMPLATE.md) for companies and security professionals.
- Detailed [evidence classifications and review rules](SCORING.md).
- A defined [public response route](responses/README.md).
- Reviewer analysis kept separate from original submissions, including the [cross-model comparison](reviews/model-comparison.md).
- A [provenance HOLD register](reviews/provenance-hold.md) for unresolved attribution.

AI-generated responses are conceptual research artifacts. They are not operational security assessments, corporate statements from model providers, independent validation of any architecture, or evidence that a company or product is secure or insecure.

## The Five Evidence Challenges

### 1. The Authority Test

**Can you demonstrate that every security-sensitive action within a defined system boundary requires valid authorization at the moment of execution?**

This includes actions initiated by administrators, services, automated processes and AI agents. It also includes missing, expired, revoked, excessive or incorrectly delegated authority.

A credible answer should identify:

- The declared authorization scope and its limitations.
- Positive and negative authorization tests.
- The enforcement point at the relevant resource or execution boundary.
- The behavior when authorization dependencies fail.
- Evidence that revocation affects subsequent actions.
- Independently reviewable, sanitized results.

**Weak answer:** “We use MFA, RBAC and zero trust.”

Authentication is not authorization. A policy is not proof of enforcement.

### 2. The Bypass Test

**Can a protected action reach its destination without passing through the control that is supposed to secure it?**

A control can make perfect decisions and still be irrelevant to an action that avoids it. Alternative interfaces, background workers, privileged integrations, emergency access, legacy paths and automated workflows must be considered.

A credible answer should identify:

- A bounded inventory of relevant execution paths.
- Where enforcement occurs.
- Tests of alternative, exceptional and failure paths.
- Resource-side evidence of enforcement.
- Coverage assumptions, exclusions and unresolved unknown paths.
- Independent review or reproduction of a meaningful sample.

**Weak answer:** “Our gateway evaluates every request.”

A correct security decision is not complete enforcement.

### 3. The Compromised Trust Test

**What remains protected when something you already trust becomes untrustworthy?**

The compromised component might be a dependency, build service, signing workflow, update channel, integration, identity provider, service identity, plugin, model or security tool.

A credible answer should identify:

- The affected trust boundary and potential blast radius.
- Controls independent of the compromised component’s own statements.
- Separation of build, approval, signing, release and runtime authority where applicable.
- Demonstrated detection, containment, revocation and recovery.
- Common-mode dependencies and residual exposure.
- The date, scope and result of a relevant compromise exercise.

**Weak answer:** “Our suppliers are reputable, and our updates are signed.”

Provenance and signatures are valuable, but authentic software can still behave unsafely or become compromised after verification.

### 4. The Consequence Test

**Can you independently establish what actually happened—not merely what the system reported?**

For a representative security-sensitive operation, reconstruct the requested action, applicable authority, enforcement decision, actual system consequence and final outcome. Successful technical execution does not automatically establish an authorized or acceptable result.

A credible answer should identify:

- An event-to-consequence evidence chain.
- The relevant policy version and authorization context.
- Sanitized enforcement records and system-of-record observations.
- Reconciliation of expected and observed outcomes.
- Criteria for an acceptable outcome.
- Missing, conflicting or incomplete evidence.
- Independent observation or verification where appropriate.

**Weak answer:** “The dashboard is green, and all logs are available.”

A recorded event is not necessarily a verified real-world consequence.

### 5. The Recovery Truth Test

**After a security failure, how do you prove that trustworthy operations have actually been restored?**

Recovery is more than restarting a service. It may require clean identity state, reliable evidence, removal of persistence, verified data integrity and confirmation that representative business outcomes are correct.

A credible answer should identify:

- Detection, escalation and containment evidence.
- Named decision authority and accountable response ownership.
- Evidence sources independent of compromised administrative or logging domains.
- Selection and verification of a clean recovery point.
- Measured recovery results against declared objectives.
- Verification of restored data, services and representative transactions.
- Unresolved findings, residual risks and corrective actions.

**Weak answer:** “We have backups and a disaster recovery plan.”

An operational service is not necessarily a trustworthy service.

## How the AI Models Are Being Challenged

Multiple AI models receive the same [master prompt](PROMPT.md), **MKM-GCEC-001**, asking for exactly five questions that separate security claims from demonstrated protection.

Each accepted submission records:

- Model and provider.
- Exact model version, or UNKNOWN if not exposed.
- Date, time and time zone, or UNKNOWN if unavailable.
- Why the prompt was asked.
- Prompt ID and version.
- The complete original response.
- Evidence status and declared limitations.

Model-reported metadata remains model-reported unless independently corroborated. A model’s confidence does not verify its identity, timestamp, statements or conclusions.

No model is declared the winner. Agreement between models may show convergence of framing; it does not independently validate a security doctrine, architecture or product.

## How Companies and Security Professionals Can Participate

Answer one question or all five. A smaller, well-scoped answer with credible evidence is more valuable than a broad answer with none.

For each answer:

1. State the specific claim being assessed.
2. Define the system, operating environment and threat-model scope.
3. Describe the test or assessment method and its date.
4. Include relevant positive, negative and failure-path tests.
5. Explain what actually happened, not only what was reported.
6. Identify independent observation, reproduction or review where available.
7. State exclusions, limitations and remaining UNKNOWNs.
8. Describe remediation and follow-up verification where relevant.

Use [ANSWER_TEMPLATE.md](ANSWER_TEMPLATE.md), then follow the [Public Response Guide](responses/README.md) to submit through a pull request under `responses/`.

## Evidence Safety

Participants do not need to disclose credentials, secrets, customer information, confidential architecture or exploitable procedures.

Use redacted artifacts, synthetic environments, scoped summaries or private independent verification under appropriate controls. Do not publish sensitive evidence merely to satisfy a public challenge. Pull requests and their histories are public; remove sensitive material before submission.

An honest UNKNOWN is always preferable to an unsafe disclosure or an invented PASS.

## Evaluation Scale

### DEMONSTRATED

Relevant, credible and appropriately reviewable evidence supports the specific claim within an explicitly defined scope. Actual outcomes and relevant negative or failure paths have been checked. Limitations are stated.

### PARTIAL

Evidence supports part of the claim, but material limitations, coverage gaps, unverified dependencies or missing outcome checks remain. The supported boundary is identified.

### UNKNOWN

Available evidence is insufficient to determine whether the claim holds. UNKNOWN does not imply weakness or failure.

### NOT DEMONSTRATED

The answer or supplied artifacts do not substantiate the specific claim. This is not a finding that the system is insecure; it means the claim remains unproven by the available answer.

### FAILED — Recorded Separately When Applicable

Relevant testing or credible evidence establishes that the claimed protection did not hold within the assessed scope. Missing evidence alone must never be recorded as FAILED.

Every classification applies only to the claim and scope assessed—not automatically to an entire product, model or organization. See [SCORING.md](SCORING.md) for reviewer roles, conflicts, participant replies and correction handling.

## Review Principles

- Evaluate evidence, not confidence, popularity or provider reputation.
- Do not confuse authentication with authorization.
- Do not confuse a policy with an enforcement mechanism.
- Do not confuse a log with an independently verified consequence.
- Do not confuse successful execution with an acceptable outcome.
- Do not confuse restored availability with restored security.
- Do not treat certifications as proof outside their actual scope.
- Do not treat missing evidence as proof of failure.
- Do not require participants to expose sensitive information.
- Do not require a preferred technology when equivalent evidence can demonstrate the same outcome.
- Keep original submissions verbatim; record corrections separately.
- Keep reviewer commentary distinct from participant evidence.
- Maintainer acceptance of a response is not a security certification.

## Repository Structure

```text
README.md                    Challenge navigation, purpose and public invitation
PROMPT.md                    MKM-GCEC-001 master prompt, unchanged
SCORING.md                   Evidence classifications and review governance
ANSWER_TEMPLATE.md           Response form for companies and professionals
CHANGELOG.md                 Dated document history
submissions/
  README.md                  Submission index and provenance rules
  claude.md                  Verbatim Claude response
  github-copilot.md          Verbatim GitHub Copilot response
  gpt.md                     Verbatim GPT response
  gemini.md                  Verbatim Gemini response
  kimi.md                    Verbatim Kimi response
reviews/
  model-comparison.md        Cross-model reviewer analysis
  provenance-hold.md         Unresolved attribution register
responses/
  README.md                  Public response and pull-request instructions
```

Additional submissions should be added only after their metadata and attribution have been reviewed. Conflicting provider information remains on HOLD rather than being silently corrected or assigned to a model.

## Public Invitation

To cybersecurity companies, AI developers, researchers, CISOs, security architects, engineers and security professionals:

Choose one question. Define your scope. Show what you tested. Show what failed. Show what changed. State what remains unknown.

We welcome DEMONSTRATED evidence. We welcome PARTIAL answers with clearly identified gaps. We welcome an honest UNKNOWN.

We do not need another polished claim.

**Why should we trust your model—and what independently verifiable evidence shows that this trust is justified?**

## The Challenge Principles

**SECURITY CLAIM ≠ SECURITY EVIDENCE**  
**AUTHENTICATION ≠ AUTHORIZATION**  
**CORRECT DECISION ≠ COMPLETE ENFORCEMENT**  
**LOGGED EVENT ≠ VERIFIED CONSEQUENCE**  
**SUCCESSFUL EXECUTION ≠ ACCEPTABLE OUTCOME**  
**RESTORED SERVICE ≠ RESTORED SECURITY**  
**MISSING EVIDENCE ≠ PROVEN FAILURE**  
**AI AGREEMENT ≠ INDEPENDENT VALIDATION**

Make security claims stronger than their marketing.

---

**Document history:** See [CHANGELOG.md](CHANGELOG.md).  
**Reuse terms:** No licence has yet been selected by the repository owner. Public availability alone does not specify reuse rights.