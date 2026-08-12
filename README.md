# Precise Activate

Zero-deviation agentic execution for **Grok Build**.

- Slash command: **`/activate`**
- Morph spine: **`morph-shared`** (Logic · Ration · Reason contract)
- Agents: `planner` · `implementer` · `verifier`
- Templates: `REQUIREMENTS` · `TASKS` · `PLAN` · `EVIDENCE`

**Seals (always):** `train_ok=false` · `measured_omega=false` · `G1=OPEN` · `endpointAssumed=false`

Repo root **is** the plugin root (not a nested monorepo folder).

## Install (this machine / workspace)

```bash
git clone https://github.com/Jadon-Fox/precise-activate.git
grok plugin install ./precise-activate --trust
# session skill mirror (optional, no marketplace):
mkdir -p .grok/skills && cp -R ./precise-activate/skills/morph-shared .grok/skills/morph-shared
```

From an already-attached Grok Build workspace:

```bash
grok plugin install ./plugins/precise-activate --trust
cp -R ./plugins/precise-activate/skills/morph-shared .grok/skills/morph-shared
```

## Use

In a Grok Build session:

```text
/activate
/activate ship feature X exactly as specified
```

Load morph spine when expanding/contracting prompts: skill **`morph-shared`**.

## Layout

```text
.
├── plugin.json                 # root manifest
├── .grok-plugin/plugin.json    # plugin-dir manifest
├── commands/activate.md        # /activate
├── skills/morph-shared/        # LRR morph controller
│   ├── SKILL.md
│   └── references/
├── agents/                     # planner, implementer, verifier
├── templates/                  # REQUIREMENTS, TASKS, PLAN, EVIDENCE
├── marketplace.entry.json
└── README.md
```

## Validate

```bash
grok plugin validate .
```

## Non-goals

- Does not close train_ok / measured_omega / G1
- Does not invent green evidence
- Marketplace submit is optional and out of default scope
