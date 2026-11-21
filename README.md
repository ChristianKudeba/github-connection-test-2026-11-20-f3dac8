# GitHub connection test 2026-11-20

Lean 4 formalization of the Principia project [GitHub connection test 2026-11-20](https://principia-math.com/projects/f3dac85b6a405e04cc3b1a50c1334a45). The layout follows the Palomar template.

Temporary test of production GitHub repository creation and organization OAuth approval. Contains only synthetic test content, no research claims or private data.

## Layout

- `Challenge.lean` states the advertised results with `sorry`; keep its imports to Lean core and Mathlib.
- `Solution.lean` proves the same declarations by importing the development in `GitHubConnectionTest2026/`.
- `comparator.json` lists the declarations Comparator checks between the two.
- `formalization.yaml` records the public description, provenance, authorship, automation and review status. Replace every `TEMPLATE` value.

## Checks

```text
lake exe cache get
lake build
ruby scripts/validate-formalization.rb
./scripts/verify-comparator.sh
```

Repository: https://github.com/ChristianKudeba/github-connection-test-2026-11-20-f3dac8
