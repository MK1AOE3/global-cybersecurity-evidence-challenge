# Hybrid Linear-Attention State — Evidence Track

Classification: VERIFIED-REFERENCE / VENDOR-PUBLISHED + ACADEMIC PREPRINT
Collected: 2026-11-09 | Verification runtime: Kimi (independent re-derivation)

## Scope
Four preprints on hybrid LLM architectures (softmax attention interleaved with
linear-attention / state-space layers) and the structure of their recurrent states
under serving and quantization.

| File | Paper | Source | Pages |
|---|---|---|---|
| 2603.15031v1 | Attention Residuals (Kimi Linear) | arXiv:2603.15031v1 [cs.LG] | 21 |
| 2609.38166v1 | LeapQuant | arXiv:2609.38166v1 [cs.LG] | 16 |
| 2611.01864v1 | Quantizing Recurrent LMs (LoReS) | arXiv:2611.01864v1 [cs.LG] | 30 |
| 2611.06084v1 | SEED (NVIDIA) | arXiv:2611.06084v1 [cs.LG] | 47 |

## Independent cross-check (performed 2026-11-09)
- All four PDFs parsed successfully; integrity OK.
- Attention Residuals numbers byte-verified against extracted PDF text:
  Table 3 = exactly 15 benchmarks; GPQA-Diamond 36.9->44.4 (+7.5);
  Math 53.5->57.1 (+3.6); HumanEval 59.1->62.2 (+3.1); 14 improved / 1 tie / 0 regressions;
  scaling coefficients 1.891/1.870/1.865; 1.25x compute claim; Table 1 Block 5.5d vs mHC 34d.
- Cross-paper convergence (independent groups, same structure): recurrent-state
  energy concentrates in a rank-one/low-rank component aligned with the mean value
  direction (SEED "state sink" + rank-R content; LeapQuant Compensator Tokens;
  LoReS value-axis grouping robustness on Kimi-Linear INT8 dL=0.001).

## Evidence class caveats (binding)
- All four are PREPRINTS, not peer-reviewed.
- SEED and LeapQuant throughput figures measured on NVIDIA hardware by
  vendor-affiliated or vendor-funded teams -> cite as VENDOR-PUBLISHED.
- SEED "we will release the code" is an unfulfilled commitment as of 2026-11-09.
- Numbers are quoted as-published; no independent reproduction was performed.

## Hash discipline
Reference SHA-256 digests in SHA256SUMS.txt were computed by the verification
runtime. Owner must recompute on the owner rig, GPG-sign the manifest, and only
then treat the pack as sealed. Signing keys never leave the owner machine.
