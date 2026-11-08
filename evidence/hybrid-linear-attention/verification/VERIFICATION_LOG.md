# Verification Log — Hybrid Linear-Attention Evidence Pack

Date: 2026-11-09
Verifier: Kimi (verification runtime), independent of build runtime
Method: parse all four PDFs; re-derive headline numbers from extracted text;
        cross-check structural claims across the three independent groups.

## Verdicts
| Item | Claim | Verdict |
|---|---|---|
| Attention Residuals arXiv ID | exists, 21pp, Kimi Team | CONFIRMED (independent arXiv search) |
| AR benchmark table | 15 rows; +7.5 GPQA / +3.6 Math / +3.1 HumanEval; 14/1/0 | BYTE-VERIFIED vs PDF text |
| AR scaling | 1.891/1.870/1.865; 1.25x compute | BYTE-VERIFIED vs PDF text |
| AR Table 1 I/O | Block 5.5d vs mHC 34d | BYTE-VERIFIED vs PDF text |
| SEED | 47pp, parses OK, internal tables consistent | CONFIRMED AS-PUBLISHED |
| LoReS | 30pp, parses OK; Kimi-Linear INT8 value-axis dL=0.001 | CONFIRMED AS-PUBLISHED |
| LeapQuant | 16pp, parses OK; 8-bit matches FP32 across 12 model-task pairs | CONFIRMED AS-PUBLISHED |
| Cross-paper rank-one convergence | 3 independent formulations, same structure | CONSISTENT |

## Not performed (explicit boundary)
No code execution, no kernel reproduction, no serving benchmarks re-run,
no contact with vendor systems. Vendor throughput numbers remain vendor claims.

## Sealing (owner-side, pending)
[ ] Recompute SHA-256 on owner rig
[ ] GPG-sign SHA256SUMS.txt with owner key
[ ] Commit with signed manifest
