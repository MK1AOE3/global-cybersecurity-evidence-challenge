Provenance HOLD Register

Record ID: MKM-GCEC-001-HOLD-001

Recorded: 2026-11-05

Status: HOLD — provider attribution conflicting

Operational assessment: None

Conflict

The owner supplied this response with the label DeepSeek. The response’s own embedded metadata states:

```text
MODEL / PROVIDER: OpenAI / ChatGPT
```

These labels directly conflict. The response must not be published as a DeepSeek submission or silently reassigned to ChatGPT. It remains outside the accepted `submissions/` set until the source is clarified.

Preservation Rule

The text below is preserved as supplied, apart from removing the owner’s leading “Deep seek” attribution label from the response body and recording that label here. No provider correction has been inferred.

Verbatim Response Body

MODEL / PROVIDER: OpenAI / ChatGPT
EXACT MODEL VERSION: UNKNOWN in this session — deployment version not exposed to the model
DATE AND TIME (WITH TIME ZONE): 2026-11-05; time and time zone UNKNOWN
WHY ASKED: To identify five questions that force security claims toward scoped, verifiable evidence rather than policy, certification or marketing language.

Evidence rule: A credible answer may use scoped summaries, independent attestations and stated limitations. If evidence is insufficient or cannot be safely disclosed, the honest answer is UNKNOWN, not PASS. Compliance certifications may support an answer but are not proof by themselves.

---

The Five Questions

1. The Unauthorized Action Test

Precise challenge question: For your highest-risk action—privilege change, data export, payment, tool invocation or agent action—can you show that every request is authorized at the enforcement point, deny-by-default, bound to the acting identity and context, and checked for alternate paths—not merely authenticated or covered by policy?

Why it separates real security from a polished answer: Authentication proves an identity; authorization proves whether that identity may perform this action, in this context, through this path. Many polished answers describe roles and policies but cannot show enforcement at the moment of consequence.

Evidence required: Enforcement-point inventory; authorization decision records tied to action IDs; negative tests for missing, expired, wrong-context or delegated permissions; alternate-path analysis; independent test summary; limitations statement.

Weak answer example: “We use SSO and role-based access, and we hold a security certification.”

---

2. The Bypass Proof

Precise challenge question: Can you show independent, scoped evidence that a normal user, compromised endpoint, misconfigured integration or delegated AI agent cannot bypass the control behind your strongest security claim?

Why it separates real security from a polished answer: A control that works only on the intended path is not the same as a control that resists alternate paths. This question tests architecture and independent verification, not confidence.

Evidence required: Independent adversarial assessment summary with scope and limitations; bypass-test categories; remediation and retest evidence; disclosure or exception handling; statement of what was not tested.

Weak answer example: “We have no known bypasses; we are penetration-tested annually and run a bug bounty.”

---

3. The Supply-Chain Provenance Test

Precise challenge question: For every component that can execute code or alter a security decision—dependency, build step, update channel, model, plugin or agent tool—can you show provenance, integrity verification at consumption, and a tested revocation or response path if an upstream artifact is compromised?

Why it separates real security from a polished answer: Supply-chain assurance is not a questionnaire. It requires knowing what entered the system, whether it was verified at use, and whether a compromised upstream artifact can be contained quickly.

Evidence required: Signed artifacts and verification records; dependency and update policy; provenance summaries; revocation or rollback drill results; scoped independent attestation; stated gaps.

Weak answer example: “We maintain an SBOM and send vendor security questionnaires.”

---

4. The Incident Consequence Ledger

Precise challenge question: When you report an incident as contained or recovered, can you show evidence that attacker action stopped and acceptable business outcomes were restored—not just that alerts closed, systems rebooted or logs looked clean?

Why it separates real security from a polished answer: Logs and dashboards describe signals; they do not prove consequences. Containment and recovery are outcomes, not ticket states.

Evidence required: Containment criteria and verified timeline; restoration and data-integrity checks; customer-impact and outcome metrics; independent validation summary where possible; post-incident control changes.

Weak answer example: “Mean time to resolve was 15 minutes, the dashboard is green and no exfiltration was found in the logs.”

---

5. The Human and AI-Agent Accountability Test

Precise challenge question: For high-risk actions taken by people or AI agents under pressure, can you demonstrate context-aware authorization, attributable action records, reversibility where appropriate and sampled review—so successful execution is not confused with acceptable outcome?

Why it separates real security from a polished answer: Training and policy describe intent. Accountability requires evidence that risky actions are constrained, attributable and reviewed when speed or stress pushes normal behavior aside.

Evidence required: Approval design for high-risk actions; agent identity and permission boundaries; tool-call records with decision context; separation of duties; fail-safe behavior; sampled review results; misuse-test summary.

Weak answer example: “We provide annual security training and have an AI usage policy.”

---

A. Four-Level Answer Scale

DEMONSTRATED: Scoped, relevant, independent or independently verifiable evidence shows the control or outcome works as claimed; limitations and gaps are stated.

PARTIAL: Some evidence exists, but coverage, independence, recency or linkage to the actual outcome is incomplete.

UNKNOWN: Evidence is insufficient, unavailable or cannot be safely disclosed. This is an honest non-pass, not a failure by default.

NOT DEMONSTRATED: The claim is supported only by policy, marketing, confidence or compliance certification, or available evidence contradicts the claim.

B. Favourite Question and Why

My favourite is The Bypass Proof. It forces the conversation from “we implemented a control” to “show that alternate paths do not defeat it.” That is where architecture, authorization, supply chain, agents and operations meet, and where independent evidence matters more than confidence.

C. Public Invitation

If you lead a security team, build AI agents or assess controls, publish a scoped answer: state the claim, show the evidence, name the limitations and mark the unknowns. Invite independent review. Make the evidence stronger than the marketing.

D. Three Memorable Security Non-Equalities

AUTHENTICATION ≠ AUTHORIZATION
POLICY ≠ ENFORCEMENT
LOGS ≠ VERIFIED CONSEQUENCES

Resolution Requirements

To clear this HOLD, record:

```text
Confirmed provider and runtime:
Basis for confirmation:
Original interface, export or other provenance evidence:
Correction authorized by:
Correction date:
```

Until then, the technical content may be reviewed as unresolved material, but it carries no accepted provider attribution.