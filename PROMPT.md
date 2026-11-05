MK MEDIA — GLOBAL CYBERSECURITY EVIDENCE CHALLENGE

Master Prompt

Prompt ID: MKM-GCEC-001

Prompt version: 1.0

Status: Fixed for the initial cross-model challenge

Usage Rules

1. Give the same master prompt to every participating AI model.
2. Fill only the submission-metadata fields; do not tailor the question to a provider.
3. Use UTC where possible. Write `UNKNOWN` rather than guessing a model version, time or time zone.
4. Preserve every response verbatim in its own file under `submissions/`.
5. Keep reviewer analysis separate from the original response.
6. Treat model-reported metadata as model-reported unless independently corroborated.
7. Treat every response as a conceptual research artifact—not a corporate statement, operational assessment or validation of a security architecture.

MKM-GCEC-001 — Verbatim Prompt

```text
MK MEDIA — THE GLOBAL CYBERSECURITY EVIDENCE CHALLENGE
Prompt ID: MKM-GCEC-001 | Version 1.0

MODEL / PROVIDER:
EXACT MODEL VERSION:
DATE AND TIME (WITH TIME ZONE):
WHY ASKED: To discover which five questions can challenge cybersecurity companies and security professionals to demonstrate real protection—not merely repeat policies, certifications or marketing claims.

You are participating in a vendor-neutral public research challenge. We are asking multiple AI models the same prompt to compare how each one identifies the gap between security claims and demonstrated protection.

Your task:

If you could ask every cybersecurity company, AI developer, security researcher, CISO and security engineer only FIVE questions, which questions would be hardest to answer without genuine evidence?

Create exactly five questions covering different security failure modes. Consider architecture, authorization, bypass paths, supply-chain compromise, human behavior, incident response, recovery, AI-agent actions and independent verification. Do not force every category into the answer; choose the five questions you believe are strongest.

For each question, provide:

1. A short, memorable title.
2. The precise challenge question.
3. Why it separates real security from a polished answer.
4. The evidence required for a credible answer.
5. One example of a weak answer that does not satisfy the challenge.

Rules:

• Challenge the industry without accusing any company of failure.
• Do not promote a product, vendor, framework or AI model.
• Do not invent incidents, statistics, certifications or technical findings.
• Compliance certifications may support an answer, but are not proof by themselves.
• An answer must not require credentials, customer information, confidential architecture or exploitable details.
• Distinguish authentication from authorization, policy from enforcement, logs from verified consequences, and successful execution from acceptable outcomes.
• Use UNKNOWN when evidence is insufficient. An honest UNKNOWN is better than an invented PASS.
• Make the language bold, intelligent and constructive—not theatrical, insulting or fear-based.

Finish with:

A. A four-level answer scale: DEMONSTRATED, PARTIAL, UNKNOWN and NOT DEMONSTRATED.
B. Your favourite question and why it matters, in no more than 60 words.
C. A short public invitation encouraging companies and security professionals to answer.
D. Three memorable security non-equalities, such as:
   SECURITY CLAIM ≠ SECURITY EVIDENCE

The objective is not to make security professionals look weak. It is to make security claims stronger than their marketing.
```

Submission Record

Complete this record for each model response. Keep this administrative record outside the verbatim response when the response is moved into `submissions/`.

```text
PROMPT ID: MKM-GCEC-001
PROMPT VERSION: 1.0
SUBMISSION FILE:
MODEL / PROVIDER:
EXACT MODEL VERSION: [MODEL-REPORTED / OWNER-REPORTED / UNKNOWN]
DATE AND TIME (WITH TIME ZONE): [MODEL-REPORTED / OWNER-REPORTED / UNKNOWN]
WHY ASKED:
RESPONSE RECEIVED DATE:
RESPONSE SOURCE: [Owner paste / export / other identified source]
VERBATIM PRESERVED: [YES / NO — explain]
METADATA CONFLICTS: [NONE / describe and place on HOLD]
EVIDENCE STATUS: Conceptual research response; not an operational security assessment
REVIEWER NOTES FILE:
```

Integrity and Attribution Note

A model’s response is evidence of what that runtime generated, not evidence that its claims are true. Agreement between models may show convergence of framing; it is not independent security validation. Conflicting provider or model metadata must remain on `HOLD` until resolved without silently rewriting the original response.