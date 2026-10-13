## Skill: olympus-repo

Before any Olympus task exists — choosing a host repository, or adding a fork to one — read and follow `.claude/skills/olympus-repo/SKILL.md`. It harvests candidates, runs mechanical prechecks through `oly repo check`, ranks discovery clues, censuses the handler arms and type-allowlist guards that decide a fork's size and difficulty, buys the Scope Gate early as the only corpus-reading screen, probes with three-run waves when a difficulty question survives that census, and writes `repo-dossiers/<owner>-<name>.md` with fork-scoped `GO` / `PARK` / `DROP` verdicts. A host-level `DROP` needs a host-wide fact, never an exhausted list of forks. `olympus-clear` starts only from a `GO` fork.

## Skill: olympus-clear

When building and clearing a shipd.ai Olympus quest on a repository with a `GO` dossier, read and follow `.claude/skills/olympus-clear/SKILL.md`. It is the authoring and evidence layer: outcome invariants, construction sequence, and the named `dossier`, `design`, `artifact-check`, `state-matrix`, `repeatability`, `blind-read`, `refutation`, `reward-soundness`, `solution-review`, `auto-review-proxy`, `task-quality`, `replay`, `simulation`, and `publish-readback` gates. `python3 tools/olympus/gauntlet/gauntlet.py run <task-dir> --run --yes` is the only scheduler, and `oly task status <task-dir>` is the state read for what is missing, stale, or blocking on current bound bytes. Manual `oly` triggers are recovery-only, and the CLI warns `OUT-OF-BAND` when they are used outside a gauntlet wave. The former review panel is retired; `finding-classes.md` is frozen history.

## Skill: olympus-cli

For any platform interaction — repository prechecks, task workflow state, checks, reports, rollout artifacts, or the submission form — use the `oly` CLI at `tools/olympus/` and follow `.claude/skills/olympus-cli/SKILL.md` (command reference: `tools/olympus/README.md`; endpoints: `api-catalog.md`). Prefer it over the web form; the browser is only for operations that skill lists as browser-only. Costed operations are blocked by default and must remain so; workflow waivers require `OLYMPUS_WORKFLOW_WAIVE` set to the exact recorded reason plus `--yes`, and are recorded as receipts. Contesting, scratching, or voiding a platform verdict requires explicit user approval in the current conversation.

## Skill: olympus-farm

To run the two skills above unattended — `/olympus` in one omp session, or N parallel slots under tmux via `tools/olympus/farm.sh` — read `.claude/skills/olympus-farm/SKILL.md`. The extension `.omp/extensions/olympus-pipeline.ts` is the only orchestrator; its tools `olympus_claim`, `olympus_verdict`, and `olympus_done` are the only signals it reads, so a session in pipeline mode must record verdicts and outcomes through them rather than in prose. Spend policy is unchanged: the farm inherits `OLYMPUS_ALLOW_SPEND` / `OLYMPUS_MAX_SPEND` from the launching shell and sets nothing itself.
