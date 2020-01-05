# Proference Motivation Doc

## Context

### Related works

- [MagicHaskeller](http://nautilus.cs.miyazaki-u.ac.jp/~skata/MagicHaskeller.html)
- [djinn](https://hackage.haskell.org/package/djinn)
- [exference](https://hackage.haskell.org/package/exference)
- ...

## Definitions

XYZZY: Tests, signatures, functions and data types to use, literals, specific compositions...

## High-level goals

### Interactive notepad-like design.

- Ideally linear progression of small increments.

- Focus on a single increment a time.

- Rely on refactoring tools to factor the sketch once satisfied.

### Work on alternatives concurrently.

Share resources between them according to likelihood of success.

For example, heuristics of resolution can be:
- Working from signature to implementation (djinn, exference)
- Working from test cases to implementation (MagicHaskeller)
- Likelihood of implementation given prior patterns in codebase
- ...

### Provide insight, present meaningful choices.

The algorithm is not omnipotent. The user should be able to get feedback on search state, and control paths.
For example, the user can instruct the prune obviously bad search spaces, or encourage searching a promising path with higher priority.

### Commit to final resolution as late as possible.

XYZZYs relating to an increment can be input separately, but are resolved together.
For example, ambiguity in tests might be resolved by further constraints, or vice-versa.


## Breadcrumbs

