# Structural Explainability: Neutral Substrate

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
![Build Status](https://github.com/civic-interconnect/NeutralSubstrate/actions/workflows/ci.yml/badge.svg)
[![Check Links](https://github.com/civic-interconnect/NeutralSubstrate/actions/workflows/links.yml/badge.svg)](https://github.com/civic-interconnect/NeutralSubstrate/actions/workflows/links.yml)

> Lean 4 formalization of the Ontological Neutrality Theorem.

## Theorem

An ontology is neutral if and only if it contains no causal or normative primitives.

```lean
∀ S : Ontology, Neutral S ↔ containsCausalOrNormative S = false
```

## Domain Scope

This formalization applies to substrates optimized for:

- Stability under durable interpretive disagreement
- Accountability across jurisdictions
- Interoperability without semantic consensus

## Paper (Submitted)

Case, D. M. (2025). "The Ontological Neutrality Theorem: Why Neutral Ontological Substrates Must Be Pre-Causal and Pre-Normative."

## Verify

```bash
lake update
lake build
lake exe neutralsubstrate
```

## Documentation

- [Paper to Lean Mapping](./docs/MAPPING.md)
- [Lean 4 Quick Reference](./docs/LEAN.md)

## Project Structure

| Item         | Value                                            |
| ------------ | ------------------------------------------------ |
| Project name | `NeutralSubstrate`                               |
| Namespace    | `StructuralExplainability`                       |
| Library      | `StructuralExplainability`                       |
| Executable   | `neutralsubstrate`                               |
| Main proof   | `StructuralExplainability/NeutralSubstrate.lean` |

## License

[MIT](./LICENSE)
