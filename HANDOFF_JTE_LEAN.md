# Next session: another JTE task, leanly

## Goal and boundaries

Create a genuinely different Olympus task on **https://github.com/casid/jte**, pinned base **`a271c27d21447fbfce3e91b2e59491e3855998ac`**, in a new `maitrish_tasks/<slug>/` folder. Deliver `description.txt`, `test.patch`, `solution.patch`, and `Dockerfile`, plus necessary execution helpers. Aim for a coherent feature naturally requiring 250+ substantive production LOC and roughly 4–5 solves in ten Luna-high attempts—not difficulty through omissions or LOC padding. No new candidate is selected yet.

The user explicitly wants brevity: reuse known facts, avoid dossier/design/review-panel bookkeeping, local LLM review stacks, and automatic repetition marathons. Keep the contract and short evidence summary in chat where possible. **Shared skills and repository instructions have not been changed.** This handoff records that preference, not a waiver of mandatory instructions, CLI guards, or paid-operation approvals. If mandatory workflow conflicts, identify the specific conflict before adding ceremony; never fabricate clearance or silently bypass guards.

## Hard exclusion: previous task is stopped

`maitrish_tasks/lean-jte-callee-defaults/` / platform draft `kh7axcj171tn0t7vmbr24d2r4n8es33m` was rejected by the user-run Scope Gate: **181/262 discounted solution lines (69.1%)** reproduced an older Java/Kotlin callee-side omitted-default dispatcher; **CLAUSE-ELABORATION** applied. Upstream and repository checks had no independent blocker. The fork is DROP, **not the repository**.

Do not repackage suppliedness transport/masks, callee-side defaults, lazy/dependent defaults, absent-versus-null maps, cross-language default scoping, or compatibility/content/varargs clauses around that engine. Originality concerns the implementation mechanism, not fresh prose or extra policies. GitHub searches did not reveal the private-corpus overlap.

The user stopped the attempt. Remaining candidate containers were stopped; artifacts and draft were preserved. No contest, scratch, void, or submission was performed. Ten VM runs were picked up, but **no final ten-run success rate was collected**. Do not resume that wave or claim calibration from it.

## Lean working loop

1. **Find a different engine.** Inspect only relevant source; use at most two narrow scouts if useful. Set one brief, explicit outcome contract before implementation. Reuse repository/environment knowledge rather than rediscovering it.
2. **Build the four artifacts.** Once the contract is fixed, implementation and behavioral verification can run concurrently with separate file ownership. One integrator exports and exercises the actual patches. Prefer additive hidden-test files; edits to existing test files can conflict with solver patches.
3. **Prove the bytes once.** Run artifact-check, then clean four-state execution: base tests pass without/with solution; new tests fail meaningfully without solution and pass with it. Check JUnit, permissions, patch applicability, and the real memory/network envelope. Fix concrete failures. Do not default to 24 repeats or speculative edge-case expansion after green results; use additional checks only when required or evidence warrants them.
4. **Screen originality early.** Fill and read back a draft once concrete artifacts exist. Obtain platform Scope Gate before expensive solver waves or polish; the user can run it. Costed CLI calls require fresh explicit approval. A derivative rejection means stop that fork, not append more clauses to the same engine.
5. **Measure only viable artifacts.** Use a small VM pilot if useful, then the required final calibration. Freeze inputs during a wave. Distinguish solver failures from infrastructure faults. Read back final form bytes; do not submit without authorization.

Lightweight static check:

```sh
bash .claude/skills/olympus-clear/gates/gate-run.sh \
  maitrish_tasks/<new-slug> artifact-check
```

That check previously took about one second; JVM execution takes minutes. The old 24 repetitions cost approximately 25 minutes. Do not confuse a direct check with completion of the full workflow ledger.

## Reuse infrastructure, not the rejected solution

Start with the old folder’s `Dockerfile`, `setup-image.sh`, `test.sh`, and `sim/Dockerfile`. Adapt test selectors and helpers; do not inherit old fixture names or its six-test baseline-count difference.

- Host Java/Maven were unavailable; Docker already solves this. Build from a pristine pinned archive, never the dirty golden workspace.
- Cache `/opt/m2repo`; test the reactor with **`-pl jte-kotlin -am`**. Omitting `-am` can silently test against an installed base generator JAR.
- Reuse final JVM limits in the Dockerfile. Golden base+new passed network-disabled as UID4242 under **1 GiB**, peak **874,033,152 bytes**, with no OOM events. Earlier larger heaps OOMed the full reactor despite passing a Kotlin-only smoke.
- Preserve writable cache/worktree permissions; remove bootstrap target directories. Public generated-package fixtures must actually be accessible. Compilation/classpath mistakes are not valid feature failures.
- Export patches through real `git diff --no-ext-diff --binary HEAD -- <complete-path-list> > file.patch`; include new files with intent-to-add. Tool presentation text is not patch bytes. A clone does not contain uncommitted edits: apply exported patches to pristine base and run them.

## VM discipline

Solver simulations run **on the VM**, not locally. Local deterministic Docker tests are fine. Resolve alias `gcp` through `.claude/skills/olympus-clear/sim/machines.local.conf`; use canonical `sim/dispatch.sh` and its current help. Do not guess project/zone.

Dispatch requires committed, upstream-identical inputs. Root history contains unrelated unpublished/divergent work: **no blanket push, pull, reset, or force-push**. The prior task used a separate remote-based partial clone to publish only simulation inputs.

Verify actual queue claims, matching containers, and growing `events.jsonl`; status output previously showed stale queue counts. `result.txt` can precede grading: completion needs `base_exit` and `new_exit`, or a diagnosed terminal fault. Pass requires both exits zero. Do not count early dispatcher P/F labels.

## Focused reading

Read selectively, not a corpus sweep:

- `.claude/skills/olympus-clear/writing-guidance.md` — outcome-only, fair prompts without implementation roadmaps.
- `.claude/skills/olympus-clear/harness/contract.md` — executable base/new runner, JUnit and real failure semantics.
- `.claude/skills/olympus-clear/reference/platform.md` — only **Criteria and readiness**, **Rollout and replay discipline**, **Resource envelope**; live platform criteria remain authoritative.
- `corpus/rubrics/taskQuality.json` and `corpus/rubrics/verifyFairness.json` — evaluation criteria, not extra local review choreography.
- `corpus/classes/tests-and-harness/originality-is-judged-on-the-golden-s-engine-against-a-corpus-we-cannot-see-novel-policy-around-a-familiar-engine-is-derivative-overlap.json` — engine-level originality lesson; ignore references to the retired review panel.
- `.claude/skills/olympus-cli/SKILL.md` and `tools/olympus/README.md` — consult when binding, filling, checking, or reading back platform state. Keep cost protections enabled.
