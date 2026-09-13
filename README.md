# MANIFEX Engineering-to-Evidence Pipeline v1

Clone-based successor of `Evank253/MANIFEX` / `manifex-genesis-runtime`.

The original MANIFEX repository is **not modified**. This repo copies that tree into `upstream/` and builds the qualification pipeline beside it.

## Protected inputs

- Original source: `Evank253/MANIFEX` @ `manifex-genesis-runtime` / `b231f11b`
- Original zip SHA-256: `35de96443caa764ae41868455ec723dc8fa335a487fc0eeff6a7ed950824d425`
- KCN Security Fabric snapshot SHA-256: `962e362c95d504fccc8b47160099c73cd7be764adc3953175e1d8003790ef1de`

## Run

```bash
PYTHONPATH=. python3 -m pytest tests/test_pipeline_qualification.py -q
```

## Evidence rule

Agent `claimed_pass` is recorded and ignored. Promotion requires execution, replay match, provenance match, and an independent verifier. Missing work is `NOT_MEASURED`. Unavailable inputs are `BLOCKED`.
