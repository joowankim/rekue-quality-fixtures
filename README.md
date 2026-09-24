# Rekue quality URL fixtures

Synthetic HTML documents for the Rekue quality corpus. They contain no personal data. The initial six source assets and expected hashes are tracked in `rekue/evaluation/assets/asset-register.jsonl`.

The `h2-url-*.html` files belong to the separately captured heldout-v2 evaluation. Their source bytes are registered in `rekue/evaluation/heldout-v2/assets/register.jsonl`; their model-processing failure remains part of that evaluation record.

The three `h3-url-*.html` files are new, unreviewed heldout-v3 inputs. Their byte hashes are preregistered in `rekue/evaluation/heldout-v3/assets/register.jsonl`. They are not captured Sources, human gold, or quality scores until Rekue verifies the public Pages response and imports it through the actual URL path. GitHub Pages serves these files only after this change reaches the configured publishing branch.
