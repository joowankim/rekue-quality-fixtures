# Rekue quality URL fixtures

Synthetic HTML documents for the Rekue quality corpus. They contain no personal data. The initial six source assets and expected hashes are tracked in `rekue/evaluation/assets/asset-register.jsonl`.

The `h2-url-*.html` files belong to the separately captured heldout-v2 evaluation. Their source bytes are registered in `rekue/evaluation/heldout-v2/assets/register.jsonl`; their model-processing failure remains part of that evaluation record.

The three `h3-url-*.html` files are new, unreviewed heldout-v3 inputs. Their byte hashes are preregistered in `rekue/evaluation/heldout-v3/assets/register.jsonl`. They are not captured Sources, human gold, or quality scores until Rekue verifies the public Pages response and imports it through the actual URL path. GitHub Pages serves these files only after this change reaches the configured publishing branch.

The three `h4-url-*.html` files are synthetic heldout-v4 inputs. Their exact bytes are preregistered in `rekue/evaluation/heldout-v4/assets/register.jsonl`. The user approved the evaluation composition, not Source-level gold. Publication alone is not a Rekue URL capture, model judgement, human browser result, or quality score; Rekue must verify the served bytes and import each page through its URL path. GitHub Pages serves these files only after this change reaches the configured publishing branch.
