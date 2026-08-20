# annual-reviews

An annual review should connect claims to evidence across the full review period. This skill produces manager and self-review drafts that leave unsupported specifics visible, plus an audit that finds evidence and rubric risks before delivery.

It produces:

- **Manager Review Draft** (A. Manager draft): built from evidence notes, role expectations, review period, and rating rubric.
- **Self-Review Draft** (B. Self-review): built from the user's evidence notes, role scope, and required form.
- **Annual Review Audit** (C. Audit): built from an existing review and any supplied rubric.

It executes the [Annual Reviews playbook](https://www.andrewluxem.com/playbooks/annual-reviews). The playbook teaches the framework. This skill runs it and returns a working artifact.

**Static by construction: no dependencies, executable code, telemetry, network calls, remote instructions, auto-update, scheduled work, or background behavior.** It reads only the files in its own skill folder. Nothing happens until a user or agent invokes it.

## Install

Clone and copy the skill into Claude Code:

```bash
git clone https://github.com/andrewluxem/annual-reviews.git
cp -r annual-reviews/skills/annual-reviews ~/.claude/skills/
```

Or install it as a Claude Code plugin:

```text
/plugin marketplace add andrewluxem/annual-reviews
/plugin install annual-reviews@annual-reviews
```

For clients that install from an archive, keep using the versioned [annual-reviews v1.0.0 ZIP](https://www.andrewluxem.com/downloads/annual-reviews-v1.0.0.zip).

## Invoke it

```text
Draft this annual review from my evidence notes
Draft a manager review from these notes. The review period is January through
Polish this annual review. They are always reliable and have a great attitude.
```

Naming the skill is always valid: `use the annual-reviews skill`.

## Files

```text
.claude-plugin/
  plugin.json
  marketplace.json
skills/annual-reviews/
  SKILL.md
  meta.yaml
  LICENSE.md
  assets/
  references/
README.md
LICENSE
```

The complete canonical package is copied under `skills/annual-reviews/`, including every asset, reference, example, and license file present in the source.

## Versioning

Plugin installation is version-pinned. When behavior changes, update the version consistently in `SKILL.md`, `meta.yaml`, and `.claude-plugin/plugin.json`, then add a changelog entry. Reinstalling is an explicit update; this repository never auto-updates itself.

## License

MIT. See [LICENSE](LICENSE). The canonical skill folder carries the same authorization in [skills/annual-reviews/LICENSE.md](skills/annual-reviews/LICENSE.md).

---

## More playbooks

This skill packages one playbook from the free library at [github.com/andrewluxem/playbooks](https://github.com/andrewluxem/playbooks). Every playbook is free to read, with no email required.
