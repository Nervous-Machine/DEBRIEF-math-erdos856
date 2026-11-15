# DEBRIEF-math-erdos856

A DEBRIEF mission record (protocol https://github.com/Nervous-Machine/DEBRIEF) for **The claimed solution of Erdős Problem #856 (sets with no k elements sharing a pairwise least common multiple)**.

This claim is on the public claims board, https://math-board.nervousmachine.com, which shows its stage, who has contributed, and what it needs next.

**Standing.** Certified 0. Accepted 0. Refuted 0. Open gaps 3. This record is at tier zero: the claim and its public artifacts are pinned, the checks still owed are listed, and nothing has been run or read yet. The first contribution is open.

## The problem

For k at least three, let f_k(N) be the largest possible sum of 1/n over a subset of the integers one to N that contains no k elements with the same pairwise least common multiple. Estimate f_k(N). Erdős gave an upper bound of order log N over log log N; Tang and Zhang in 2025 showed f_k(N) lies between two powers of log N with exponents strictly between zero and one, exponents tied to the sunflower conjecture.

Source: https://www.erdosproblems.com/856 (posed: Erdős (1970)).

A third-party formalization of the problem statement exists: `FormalConjectures/ErdosProblems/856.lean` in github.com/google-deepmind/formal-conjectures at commit `e028240a61822d970c933f4656f51da025cf200b` (blob `9f1f0161ebe0c46662d6dcda4987535dd001d6cc`). It is the natural reference for whether a claimant's Lean theorem states this problem.

## The claim

**RayYoung, Keheng Zhu and Yanping Luo**, using GPT 5.6 Sol Pro (as listed by the claimants), submitted 2026-07-18 at https://www.erdosproblems.com/forum/thread/856/proof-claims.

The claim is that f_k(N) equals (log N) to the power gamma_k plus o(1), where gamma_k is a supremum over finite block parameters of a quantity built from the largest r-uniform family on n points with no k sets sharing the same pairwise union. Matching weighted upper and lower bounds reduce the problem to that finite extremal formula. The authors say the proof is short, that they checked it themselves and uploaded it after minor revisions without a Lean formalisation, and that it builds on the existing literature and the problem's discussion thread.

Artifacts, pinned:

- an Overleaf document (read link): https://www.overleaf.com/read/smhxdxnrmkbs#0eb184

Status on the problem page as of 2026-11-14: listed as one proof claim; not marked accepted by the site.

## What is owed

Each open gap is in `ASKS.md` with what closes it and who could act. In order:

1. **No formal deduction exists for the claimed proof** (EG1): A formalization of the main theorem, with the statement written by someone other than the prover.
2. **No independent mathematician has reported reading the proof, and there is no referee report** (EG2): Someone in the field reads it and says, under their name, what holds and what does not.
3. **The write-up is not a fixed file** (EG3): the authors post the write-up as a fixed file or an arXiv preprint

## Contributing

- **Rerun** (if there is a Lean development): copy `prereg_rerun.yaml`, fill in your predictions, register it with `tools/prereg.py register` from the protocol repository and commit it *before* running anything. Run. Report with the **Rerun report** issue form; it becomes a `rerun` cycle under your name.
- **Read**: a trace (reading guide) does not exist yet. Writing one is itself a `trace` cycle. Once it exists, the **Semantic read** form takes signatures and refusals.
- **Anything else**: open a plain issue.

Rules and templates: https://github.com/Nervous-Machine/DEBRIEF/blob/main/CONTRIBUTING.md. Every contribution is one dated cycle under your own name and goes into `CITATION.cff` and the next release.

## Layout

```
ledger/erdos856.json   the ledger (protocol 0.1.0)
claim.yaml            the pinned claim this record was opened from
SCORECARD.md / ASKS.md  generated from the ledger
prereg_rerun.yaml     a pre-registration template for the first rerun (unregistered)
cycles/               contributed cycles, one file each
```

## Words

This record never calls the claim proved, verified or a theorem. It records what was claimed, what was checked by whom under what rule, and what is still open. Nothing here has standing until a cycle gives it one.
