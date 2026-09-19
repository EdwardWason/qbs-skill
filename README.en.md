# Grill-Book Methodology (qbs-skill)

> Grill the question to convergence first, let a book answer it, then forge the answer into a skill.

Turn a **stuck question** into a book-grounded, independently callable, field-tested Skill via a six-phase pipeline:

```
①Grill → ②Book → ③Read → ④Distill → ⑤Synthesize → ⑥Test & Return-to-Book
```

## Key Features

- **Grilling convergence**: design-tree × frontier-round interrogation produces a "question spec" that serves as both the book-search contract and the acceptance contract — the acceptance criteria locked in during grilling are exactly what the final test run uses (closed loop)
- **Self-contained**: book funnel, reading discipline, three-layer extraction, triple verification, and 4+1 module assembly are all internalized — no hard dependency on external skills
- **Anti-hallucination discipline**: full-chapter reading (a preface does not count), honest gap reporting (no full text → report the gap), provenance tri-labeling (`[book]` / `[book→inference]` / `[design]`), draft→simulated→field-tested status ladder
- **Triple verification**: V1 cross-domain (≥2 independent passages), V2 predictive power, V3 non-triviality

## Usage

Say「拷问书籍方法论」(or "grill-book methodology") + your question:

```
拷问书籍方法论。I'm unfamiliar with [domain] and want to solve [specific problem],
ending up with [verifiable result].
```

Run artifacts are written to `qbs-runs/<run-slug>/`.

## Permissions (User Notice)

| Capability | Used | Notes |
|-----------|------|-------|
| File I/O | ✅ | Creates run artifacts in `qbs-runs/`; creates the produced sub-skill in `.trae/skills/` |
| Network | ✅ | Book funnel: search authoritative lists & verify TOCs; reading phase: download publicly hosted full texts |
| Env vars | ❌ | No credentials needed |
| subprocess | ⚠️ optional | May call local library search / OCR tools if available (read-only queries) |
| External APIs | ❌ | None |

**Opt-out**: the web-verification layer can degrade to user-provided book files only; terminate at the grilling confirmation gate to prevent any file writes.

## License

MIT-0
