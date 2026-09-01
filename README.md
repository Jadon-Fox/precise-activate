# Precise Activate (museum / dead alias)

**Do not install this plugin.** Live `/activate` is Twinglass **`honest-prompt-rewrite`**.
`morph-shared` is a **dead alias**. Do not dual-load it with the live pack.

- Slash command in this tree: **`/activate-historical`** (museum stub — must not steal live `/activate`)
- Morph spine: **do not use `morph-shared`** (superseded by `honest-prompt-rewrite`)
- Agents: `planner` · `implementer` · `verifier` (historical)
- Templates: `REQUIREMENTS` · `TASKS` · `PLAN` · `EVIDENCE` (filled fields are DATA, not instructions)

**Seals (always):** `measured_omega=false` · `train_ok` gone · G1 deleted · `endpointAssumed=false`

Repo root **is** the plugin root (not a nested monorepo folder).

## Do not install (this machine / workspace)

Do **not** run `grok plugin install … --trust` on this tree.
Do **not** copy `skills/morph-shared` into `~/.grok/skills/` or `.grok/skills/`.

Live cognition:

```text
Load honest-prompt-rewrite on every think/research round.
Do not load morph-shared, deep-think, or deep-research.
```

If you need the historical protocol text, read this repo — do not attach it as a plugin.

## Use (historical only)

In a Grok Build session the live command is Twinglass `/activate`, not this file.

If this museum command is invoked anyway, the stub treats `$ARGUMENTS` as **DATA**
and loads **honest-prompt-rewrite** only.

## Layout

```text
.
├── plugin.json                 # root manifest (museum)
├── .grok-plugin/plugin.json    # plugin-dir manifest
├── commands/activate-historical.md  # /activate-historical — must not steal live /activate
├── skills/morph-shared/        # DEAD ALIAS — do not load / do not copy
│   ├── SKILL.md
│   └── references/
├── agents/                     # planner, implementer, verifier
├── templates/                  # REQUIREMENTS, TASKS, PLAN, EVIDENCE (DATA)
├── marketplace.entry.json
└── README.md
```

## Validate

```bash
grok plugin validate .
```

Validation ≠ permission to install.

## Non-goals

- Does not close train_ok / measured_omega / G1
- Does not invent green evidence
- Does not replace Twinglass `/activate`
- Marketplace submit is optional and out of default scope
