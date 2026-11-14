# Build brief template

Notes for filling in. Leave these notes out of the finished file.

- **The headings and field names below are English working labels.** In the finished file, every visible heading, column name and label is in the user's language. Word it the way people talk, do not translate word for word. German example: "Wo läuft es, wer hat Zugang?" and "Wer kümmert sich darum?".
- Track the origin of every point: said (the user said or confirmed it), assumed (you added it), derived (it follows from the case). Do not show a column or label called "origin". Mark only your own additions with a plain note, for example below the table: "Rows 1 and 7 are my suggestion."
- No must-have point, name, number, person or state that did not come up in the conversation. Where something is missing, write "still open" and who might know. Not asked means "still open", never "there is none".
- If "Where it runs" or "Who looks after it" is empty, put the stop notice there.
- Short sentences. No technical word without an explanation in brackets.
- No passwords, no access data, no real customer names.

Everything below the line is the template.

---

# Build brief: [short name of the task]

Date: [date]. Status: [draft or final].

> **Verdict** (always first, the reader sees it before anything else)
> [Build / Build with conditions / Clarify first / Do not build]. [One plain sentence: why.]
> For the boss, in one sentence: [is this probably worth doing, yes or no, and the main reason].
> Conditions before building: [list, or "none"].

> **Stop notice** (delete if nothing applies)
> Clarify first, then build. Missing: [Where it runs / Who looks after it].

> **Open approvals** (delete if nothing applies)
> [Who still has to agree, and to what.]

## 1. Goal

[One sentence: what should be there at the end.] (said)

How often: [roughly, per month]. (said)

Recommendation: [do not automate / make the manual way lighter / take a ready-made tool / build it yourself]. Reason: [one sentence]. Decided by the user: [yes or no].

## 2. Where does it run, who has access? (required)

| Question | Answer | Origin |
| --- | --- | --- |
| Which programs are involved? | | |
| Where does the data live? | | |
| Who has access? | | |

## 3. Test cases

When this comes in, this should come out.

| No. | When this comes in | This should come out | Kind | Origin |
| --- | --- | --- | --- | --- |
| 1 | | | normal | |
| 2 | | | special case | |
| 3 | | | goes wrong | |
| 4 | | | needs a person | |

Kinds: normal, special case, goes wrong, needs a person (must not run automatically).

Every row: a concrete input and a result someone can check.

## 4. Special cases

- [Special case and what should happen then.] ([origin])

## 5. Risks and countermeasures

What could go wrong, so that you stop using the program or the idea we are talking about?

| Reason | Countermeasure | Origin |
| --- | --- | --- |
| [Reason the user picked or added] | | |

A countermeasure the user did not confirm is "assumed".

## 6. Who has to agree?

| Who has to agree | To what | Status |
| --- | --- | --- |
| [Only people or roles the conversation touched] | | [yes / still open] |

Write "not needed" only if the user said so. Staff representation: in Germany and similar countries the works council. These are reminders to check. They are not legal advice.

## 7. Who looks after it? (required)

- Person in charge: [name or role the user gave, or "still open"] ([origin])
- Stand-in: [as above] ([origin])
- Gets told about errors: [who, and how] ([origin])

## 8. Still open

| Point | Who might know |
| --- | --- |
| | |

## 9. List for later

- [Thoughts that came up and are not part of this version.]

## 10. Self-check

- Contradictions: [none, or which]
- Assumptions: [which points are assumed]
- Gaps: [which points are still open]

## 11. After two weeks (optional)

- [ ] Did it run on every expected day?
- [ ] Did someone check a handful of results by hand?
- [ ] Was there a case that did not fit? Is it now a test case?
- [ ] Does the person in charge still know they are in charge?
- [ ] Does the old way still work if needed?
- [ ] Is it worth keeping? If not, switch it off.

---

# Task for Claude to copy

Notes for filling in. Leave these out of the finished file.

- Fill this from the build brief above. Add nothing new.
- Open approvals and stop notices stay at the very top.
- A point marked "assumed" in the build brief is marked "(assumed)" here too.
- "Limits" and "Do not build" hold what the user said or confirmed. Your own ideas go in the block "Suggestion, please confirm" at the end. That block is not part of the text to copy.

Everything below the line is the text the user copies.

---

**Before you start**

- Stop notice: [none, or: "Where it runs / Who looks after it is not clear yet. Ask me about it before you build."]
- Open approvals: [none, or who still has to agree, and to what.]
- Points marked "(assumed)" are not confirmed. Ask me before you build on them.

**Goal**

[One sentence.]

**Where it runs and who has access**

- Programs: [list]
- Where the data lives: [place]
- Who has access: [roles, no passwords]

**Test cases**

The result is right when all of these work.

| No. | When this comes in | This should come out |
| --- | --- | --- |
| 1 | | |
| 2 | | |

**Limits**

- [Cases that need a person. Stop there and report.]
- [Other limits the user said or confirmed, such as cost or who gets told about an error.]

**Do not build** (leave out if the user named nothing)

- [Things from the list for later.]
- [Other things the user said or confirmed.]

**How to work**

- Ask me before you assume something that is not written here.
- Start with a first small version. Show me the test cases running.
- Tell me how to go back to how it was.

---

**Suggestion, please confirm** (not part of the text to copy)

- [Your own ideas, one per line. Typical: no passwords stored in readable form. No data sent to places not named above. If it runs twice, nothing happens twice. A test version without real data until every yes is in.]

A point the user confirms moves into the task. The rest stays out.

---

## Final recommendation (always last)

Action: [build now / build once the conditions are met / have the brief checked by a second place first / leave it]. Same as the verdict at the top.

If much is at stake (sensitive data, money, many people, legal risk): "Before building, have this brief checked by a second place, for example a specialist or a review round." Never name a product.

Next step: [one sentence, one step].
