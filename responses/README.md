Public Response Guide

This directory contains public answers to the MK MEDIA Global Cybersecurity Evidence Challenge.

1. Choose a Scoped Claim

Select one question from the [five evidence challenges](../README.md#the-five-evidence-challenges). Answer one specific claim rather than making a general statement that a product or organization is secure.

A small, well-scoped answer is preferable to a broad unsupported answer.

2. Prepare the Answer

1. Copy [ANSWER_TEMPLATE.md](../ANSWER_TEMPLATE.md).
2. Complete the metadata, claim, scope, method, evidence, limitations and self-classification.
3. Complete only the question-specific modules relevant to your answer.
4. Read [SCORING.md](../SCORING.md) for classifications, reviewer independence and correction handling.
5. Complete the publication-safety checklist.

3. Submission Route

Submit public answers through a pull request.

Recommended path:

```text
responses/<organization-or-public-alias>/<question>-<short-claim>.md
```

Examples:

```text
responses/example-org/authority-payment-approval.md
responses/example-researcher/recovery-clean-room-exercise.md
```

Use a public-safe organization name or alias. Do not include sensitive system names in the filename.

For questions, provenance corrections or review-related replies, open an issue and link the relevant response or review record.

4. Public Disclosure Safety

Pull requests, files and their revision histories are public. Before submitting, confirm that the answer contains no:

- Credentials, secrets, tokens or private keys.
- Customer information or unnecessary personal data.
- Confidential architecture.
- Exploitable procedures or sensitive exploit detail.
- Evidence you are not authorized to publish.

Use redacted artifacts, synthetic environments or scoped summaries. Private independent evidence may be referenced without being uploaded.

No confidential-submission channel is currently provided. Do not send confidential material under the assumption that private receipt or review is available.

5. Review Process

Maintainers first check submission form, scope, provenance and disclosure safety. Evidence review, if any, must identify the reviewer, method, evidence examined, independence, conflicts and limitations.

Participants self-classify. Maintainer acceptance of a pull request is an editorial decision—not security certification or endorsement.

Participants may reply, clarify scope, submit additional sanitized evidence or request a correction through a linked issue. Corrections and appeals are recorded with dated history.

6. Acceptable Outcomes

- `DEMONSTRATED`
- `PARTIAL`
- `UNKNOWN`
- `NOT DEMONSTRATED`
- `FAILED`, only where evidence establishes failure within scope
- `CLARIFICATION REQUIRED`
- `HOLD`, for provenance, safety or handling issues

Every result applies only to the claim and scope assessed.

An honest `UNKNOWN` is welcome. An unsupported `PASS` is not the objective.