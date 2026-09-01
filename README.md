# Technical Communication Skill

A bilingual Codex skill for clear, practical communication in technical work.

It helps write and edit client messages, proposals, project updates, technical explanations, decision records, and documentation in Russian or English. The skill keeps the tone direct, calm, specific, and human without tying the workflow to any marketplace, company, or individual.

Русская версия: [README.ru.md](README.ru.md).

## What it covers

- client, partner, and freelance proposals;
- technical business correspondence and follow-ups;
- project, incident, and delivery updates;
- scoped technical explanations and decisions;
- drafting and editing technical documentation;
- rewriting text that sounds generic, inflated, or machine-generated.

It is not a substitute for domain expertise, legal review, security review, or product decisions. It does not invent facts, experience, estimates, commitments, or access.

## Install

```bash
git clone https://github.com/borkli/technical-communication-skill.git \
  ~/.codex/skills/technical-communication
```

Restart Codex after installation so it discovers the skill.

## Use

Invoke the skill explicitly, or let Codex select it for a relevant writing task.

```text
Use $technical-communication to write a concise Russian update for a client:
the API migration is complete, the staging smoke test passed, and production deployment needs approval.
```

The skill responds in the language of the request unless the user asks for a translation or a different language.

## Structure

```text
technical-communication/
├── SKILL.md
├── agents/openai.yaml
└── references/
    ├── formats.en.md
    ├── formats.ru.md
    ├── rules.en.md
    └── rules.ru.md
```

`SKILL.md` contains the shared workflow and routes language-specific work to the appropriate reference. The references are deliberately separate so Russian and English conventions remain first-class rather than being mixed into one set of examples.

## Contributing and releases

Contributions are welcome through pull requests. Read [CONTRIBUTING.md](CONTRIBUTING.md) first; Russian guidance is available in [CONTRIBUTING.ru.md](CONTRIBUTING.ru.md). The `main` branch is intended to accept reviewed pull requests only.

Releases use semantic version tags at meaningful milestones. See [RELEASING.md](RELEASING.md) and [CHANGELOG.md](CHANGELOG.md).

## License

This project is released under the [MIT License](LICENSE).
