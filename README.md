## Lucas Meyer (he/him) — Berlin, Germany

Test harness engineer & edge-case investigator.  
Specializing in automated testing frameworks, fuzzing harnesses, and deterministic failure isolation.

---

### 🛡️ Test Framework Contributions & Fixes

| Framework | Area | Tracking | Status | Defect Prevented |
|---|---|---|---|---|
| **[pytest-dev/pytest](https://github.com/pytest-dev/pytest)** | Subtests Engine | Issue #15201 | `Active` | Prevents negative subtest durations when `time` is mocked |
| **[HypothesisWorks/hypothesis](https://github.com/HypothesisWorks/hypothesis)** | Property Testing | Strategy Engine | `Audited` | Integer choice constraint key collision under weighted distributions |
| **[tox-dev/tox](https://github.com/tox-dev/tox)** | Environment Matrix | Matrix Runner | `Audited` | Isolated virtualenv package resolution determinism |

---

### 🧪 Testing Principles

1. **Deterministic Assertions**: No flaky sleep timers; use monotonic clock references (`_pytest.timing`).
2. **Mutation Testing**: Verify that tests genuinely fail when production behavior is mutated.
3. **Pre-Flight Invariant Validation**: Before dispatching PRs upstream, code diffs are verified with [ZeroSlop™ CI](https://github.com/marketplace/actions/zeroslop-by-ribbsaeter-systems).

---
*Pytest • Hypothesis • Tox • ZeroSlop CI*
