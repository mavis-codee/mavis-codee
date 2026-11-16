# Koji Tamaki

GitHub: **[@mavis-codee](https://github.com/mavis-codee)**
Contact: **kojitamaki223@gmail.com**

## Lean 4 formalisation

- **[erdos-504-lean](https://github.com/mavis-codee/erdos-504-lean)** — a complete,
  sorry-free Lean 4 formalisation of the minimax angle in **Erdős Problem #504
  (Blumenthal's problem)**, submitted as `JSP-000404` to the
  [Justin Sun Prize](https://github.com/TheJustinSunPrize/awards) problem bank
  (contribution PR: <https://github.com/TheJustinSunPrize/awards/pull/5592>).

  - **Main theorem** — `Erdos504.erdos_504`: `α_{2^n} = π (1 − 1/n)`, proved
    completely in `Erdos504Formal/Erdos504Minimax.lean`.
  - **Endpoint** `α_{2^n − 1}` — `Erdos504Formal/Erdos504Endpoint.lean` proves the
    sharp (ε-relaxed) side and the supremum half `α_{2^n − 1} ≤ π (1 − 1/n)`, and
    reduces the endpoint itself to one counting lemma (`StrictCountingBound`) that is
    **stated but not proved**, so the endpoint is not claimed as formally proved.
  - **Not covered** — Sendov's complete determination of `α_N` is not formalised, and
    the mathematical-solution role is not claimed; the mathematical solution is the
    published record (Szekeres 1941; Erdős–Szekeres 1960/61; Sendov 1995) already
    recorded in the problem bank.
  - **Toolchain** — Lean `v4.33.0`, Mathlib `v4.33.0`; the audited targets depend only
    on the standard axioms `propext`, `Classical.choice`, `Quot.sound` (no `sorryAx`,
    no `admit`, no `native_decide`).
  - **Upstream file** — `Erdos504Formal/Erdos504.lean` is republished unchanged from
    [`ToshiDad/erdos-504`](https://github.com/ToshiDad/erdos-504) with its original
    authorship and original dates; see the repository's
    [`ATTRIBUTION.md`](https://github.com/mavis-codee/erdos-504-lean/blob/main/ATTRIBUTION.md).

## Attribution

Every commit in the repositories linked above was made by the account `mavis-codee`
(display name Koji Tamaki). The author address of each commit is a verified address of
this account, so GitHub attributes every commit to it. The author display name and the
commit address were updated once, after the proof history had been pushed, and **no
commit identity was ever rewritten**: the priority anchor
`a3e262e8fadde9a5b208495d94f4d71f0092d6db` and the whole submitted history keep their
original object ids, author strings and dates.
