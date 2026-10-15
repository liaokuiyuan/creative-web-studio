# Creative Web Studio

**Expert-led, intent-driven autonomous web development with mandatory seven-stage gates.**

[简体中文](README.zh-CN.md)

> Early development version. The skill is a portable instruction-and-resource bundle; it cannot grant browser, GPU, image-generation, local file or shell capabilities to a host agent that does not already have them.

## Scope

Use for creating **complete websites or web apps from scratch**, or for **comprehensive reconstruction** of an existing site. Do not invoke for isolated bug fixes, minor styling, copy edits or routine maintenance.

Seven mandatory stages apply **even to small eligible projects and template-based sites**: (1) intake and environment assessment, (2) clarification/risk analysis, (3) visible design references, project priorities, technology and asset/rendering decisions, (4) explicit user approval of a versioned intent baseline, (5) implementation, (6) evidence-based critical review and iterative regression-tested repair, and (7) honest delivery.

**A model should never quietly skip a stage.** Professional judgment and a non-sycophantic review stance apply throughout. Actual technology adoption is optional even though the *assessment* is mandatory.

## Installation

Install the repository folder as `creative-web-studio` in a location recognized by your Agent Skills-compatible host. The folder's root `SKILL.md` is the skill entry point. Follow your client's skill installation instructions; client support for resource files, shell commands and interactive widgets differs.

## Files

- `SKILL.md` — small normative controller and stage gates.
- `references/` — specialist playbooks loaded during the relevant mandatory stage.
- `scripts/normalize_weights.py` — deterministic priority normalization.
- `scripts/workflow_state.py` — local state/evidence tracker and stage checks (not authentication).
- `tests/` — Python unit tests for deterministic helpers.

## Example

User: “Build a cinematic interactive robotics showcase site with equipment pages and a functional demo.”

Agent: Evaluates scope and environment, clarifies only material unknowns, presents visible creative directions and viable technical alternatives, requests user-defined priorities, evaluates image/3D pipelines, writes an intent baseline and **waits for explicit client approval**. After approval it implements the website, runs real tests where possible, resolves identified defects with regression checks, then delivers evidence and known limits.

## Local tool tests

```bash
python -m unittest discover -s tests -v
python scripts/normalize_weights.py 'Visual design=35' 'Interaction=30' 'Functionality=25' 'Security=10'
python scripts/workflow_state.py --help
```

The tests validate *helper behavior* only. They do not demonstrate that a specific AI model fully complied with all stage requirements. Evaluating end-to-end agent behavior requires running real website projects with usable browser/build tools and independently checking outputs.

## Safeguards & limits

- No silent scope reduction, fake interactive controls, hidden placeholders, claimed-but-unrun tests or invented UE5/Blender outputs.
- For client approval, explicit consent in the conversation is required. State files may preserve its reference but cannot establish identity or authenticity.
- Protect sensitive data; do not assume arbitrary web assets are commercially usable.
- The helper can enforce **file-level ordering**, not prevent a model from ignoring its instructions when the host does not enforce them.
- Slider UI is host-dependent. Text priority selection and tested normalization are supported fallbacks.

## Licensing

A license has **not yet been selected**. Do not assume copying, redistribution or commercial reuse rights until the owner publishes a license.

## Project status

Initial engineering foundation, not a validated release. Planned next step: end-to-end behavior evaluation on representative greenfield and reconstruction projects, evidence traceability refinement, and platform compatibility verification.
