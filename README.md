# make-it-go-away

A few questions, then a build brief, or an honest no.

**Status: beta.** It works, it is small, and it has been tried on two real cases by the same person only.

## What it is

People don't want drills, they want holes. When you ask an AI to build something for your work, it often builds the drill and misses the hole. Later you find out what was forgotten: who else is affected, the odd cases, the data, the access, who looks after it, who has to agree.

`make-it-go-away` is a small add-on for AI assistants (an "agent skill", for example for Claude) that asks those questions first. You tell it about a task that keeps coming back and annoys you. It asks one plain question at a time, starting from a real case. At the end you get:

- a **verdict** at the top: build, build with conditions, clarify first, or do not build
- a **build brief**: a short written order you can build from and check against, with test cases
- a **task to copy** into a new conversation, so Claude knows what to build and where to stop
- one clear **final recommendation** with one next step

If the idea is probably not worth it, it says so early and in one sentence. Planning on then needs a reason from you, in your own words.

## Who it is for

People who are good at their work but not at writing instructions for an AI or detailed task descriptions. A carpenter, a site manager, an office worker who watched a video and wants to automate something. It uses everyday words and explains a technical term once, when it is needed. It answers in your language.

## Who it is not for

- It does not build the automation. It clarifies what should be built.
- It is not for the product descriptions of software teams ("PRDs") or for user stories (short feature descriptions).
- It is not a replacement for a specialist, a lawyer or a data protection officer.

## How to use it

1. Download this page as a ZIP file (on GitHub: the green "Code" button, then "Download ZIP"). The folder `skills/make-it-go-away` inside it is the skill.
   - In Claude.ai: open your account settings and look for the skills section. Upload the folder there as a ZIP file. The menu names can change.
   - In Claude Code: copy the folder into your skills folder (`.claude/skills/`).
   - With the command line: `npx skills add nils-bergenthal/make-it-go-away`
2. Start a new conversation and say: `Make it go away: [your problem, described briefly]`
3. Answer one question at a time. Say "result now" at any time.

Replace names and numbers before you paste anything. The conversation runs through the company behind your AI. Do not enter passwords, access data or real customer or patient data.

## Examples

Three short, invented conversations with their results, from easy to hard:

- `skills/make-it-go-away/examples/invoices.md`: invoices from emails into a table. Verdict: build with conditions.
- `skills/make-it-go-away/examples/reminders.md`: lesson reminders in a driving school. Personal data of young people, a ready-made tool that may exist. Verdict: clarify first.
- `skills/make-it-go-away/examples/thank-you-mails.md`: thank-you mails in a bike shop. Too small to plan. Verdict: do not build.

## Works with other skills

It works alongside general interview and review skills. A review round after the build brief is a good idea when much is at stake, for example with sensitive data or money.

## What we know and do not know

- It has not yet been compared with an ordinary chat in a controlled test, so there are no numbers on how much it finds that a plain request would miss.
- It has been tried on two real cases by one person, who rated it positively. It has not yet been tested with people who do not know it. If you try it, feedback is welcome. Use the feedback form under "Issues" on this page (a free GitHub account is needed), or write down your answers from `docs/test-sheet-en.md` (German: `docs/test-sheet-de.md`) and give them to whoever shared the skill with you.
- Treat the results as a starting point. A build brief lowers the chance of a miss. It does not remove it.

## Notes

- Points about data protection, contracts and staff representation are reminders to check. They are not legal advice.
- The skill reads, writes and edits files only. It runs no programs and uses no network. See `SECURITY.md`.
- Not affiliated with Anthropic or any other company.

## License

MIT. See `LICENSE`.
