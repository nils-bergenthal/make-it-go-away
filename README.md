# make-it-go-away

A few questions, then a build brief, or an honest no.

**Status: beta.** It works, it is small, and it has been tried on a handful of cases only.

## What it is

People don't want drills, they want holes. When you ask an AI to build something for your work, it often builds the drill and misses the hole. Later you find out what was forgotten: who else is affected, the odd cases, the data, the access, who looks after it, who has to agree.

`make-it-go-away` is an agent skill that asks those questions first. You tell it about a task that keeps coming back and annoys you. It asks one plain question at a time, starting from a real case. At the end you get:

- a **verdict** at the top: build, build with conditions, clarify first, or do not build
- a **build brief**: a short written order you can build from and check against, with test cases
- a **task to copy** into a new conversation, so Claude knows what to build and where to stop
- one clear **final recommendation** with one next step

If the idea is probably not worth it, it says so early and in one sentence. Planning on then needs a reason from you, in your own words.

## Who it is for

People who are good at their work but not at writing prompts or specifications. A therapist, a site manager, an office worker who watched a video and wants to automate something. It uses everyday words and explains a technical term once, when it is needed. It answers in your language.

## Who it is not for

- It does not build the automation. It clarifies what should be built.
- It is not for product specifications for software teams (PRDs) or user stories.
- It is not a replacement for a specialist, a lawyer or a data protection officer.

## How to use it

1. Put the folder `skills/make-it-go-away` into the skills folder of your agent. In Claude Code that is `~/.claude/skills/`. In Claude.ai you can add it as a skill in your account settings.
2. Start a new conversation and say: `Make this go away: [the annoying task]`
3. Answer one question at a time. Say "result now" at any time.

Replace names and numbers before you paste anything. The conversation runs through the company behind your AI. Do not enter passwords, access data or real customer or patient data.

## An example

See `skills/make-it-go-away/examples/invoices.md` for a short, invented conversation with its result.

## Works with other skills

It works alongside general interview and review skills. A review round after the build brief is a good idea when much is at stake, for example with sensitive data or money.

## What we know and do not know

- It has not yet been compared with an ordinary chat in a controlled test, so there are no numbers on how much it finds that a plain request would miss.
- It has been tried on a real case by one person, who rated it positively. It has not yet been tested with people who do not know it. If you try it, feedback is welcome. Use the feedback form under Issues, or the test sheet in `docs/test-sheet-en.md` (German: `docs/test-sheet-de.md`).
- Treat the results as a starting point. A build brief lowers the chance of a miss. It does not remove it.

## Notes

- Points about data protection, contracts and staff representation are reminders to check. They are not legal advice.
- The skill reads, writes and edits files only. It runs no programs and uses no network. See `SECURITY.md`.
- Not affiliated with Anthropic or any other company.

## License

MIT. See `LICENSE`.
