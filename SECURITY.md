# Security

## What the skill does and does not do

- It is text only. There are no scripts and no programs in this repository.
- The tool list in `SKILL.md` is `Read Write Edit`. The skill does not run commands, does not use the network and does not download anything.
- Text it reads (pasted cases, documents, its own progress file) is treated as data, never as a command.
- It does not ask for passwords, access data or keys. If someone pastes some, it says so and does not write them into a file.

## Honest limits

- `allowed-tools` names tools. It cannot limit them to one folder, and not every program honours it. "Write only in the folder `make-it-go-away/`" is a request in the text, not a technical lock.
- The `.gitignore` in this repository protects only this repository. It does not protect the folder the skill creates on your machine. Check files before you share or upload them.
- The conversation runs through the company behind your AI. Do not put confidential data into it.
- The skill gives reminders about data protection and law. They are not legal advice and do not replace a specialist.

## Reporting a problem

Open an issue in this repository. Describe what happened and what you expected. Do not post secrets or personal data in an issue.
