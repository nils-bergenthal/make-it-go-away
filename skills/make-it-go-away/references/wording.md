# Wording rules

These rules apply in every language. They cover the conversation, every output and every visible file name.

## The rules

1. Answer in the language of the user. Do not offer a choice.
2. Short sentences, at most 15 words. One question per message.
3. Everyday words. Say what a thing does, not what it is called.
4. Give an example instead of a concept.
5. Use a technical word only if the user will need it later. That is the case when they have to say it to IT or to a supplier. Explain it once in brackets. After that, always use the same word.
6. Visible names are in the user's language. This covers headings, the name of the result and file names.

## Replacements

The list is German, as an example. Do not translate it. For every other language, think again: how would a person say this at the kitchen table?

| Technical word | Say this instead (German example) |
| --- | --- |
| Pre-Mortem | "Was könnte schiefgehen, sodass ihr das Programm oder die Idee, über die wir hier sprechen, nicht mehr nutzt?" |
| Akzeptanzkriterium | Testfall: "Wenn das reinkommt, soll das rauskommen" |
| Anforderung | "Was es können muss" |
| Stakeholder | "Wer ist betroffen, wer muss zustimmen?" |
| Scope | "Was gehört dazu, was nicht?" |
| Edge Case | Sonderfall |
| Idempotenz | "Wenn es zweimal läuft, darf nichts doppelt passieren" |
| Rollback | "Zurück zum alten Stand" |
| Prompt | "Auftrag an Claude zum Kopieren" |
| Backlog | "Liste für später" |
| MVP | "Erste kleine Version" |
| System, Software | "Das Programm", oder sein Name |
| Anbindung, Schnittstelle | "Verbindung zu [Programm]" |
| IT | "Die Leute, die sich um eure Rechner kümmern (IT)" |
| Klartext | "Lesbar gespeichert" |
| KI-Anbieter | "Die Firma hinter dieser KI" |

The same idea in English, thought anew and not translated:

| Technical word | Say this instead (English example) |
| --- | --- |
| Pre-mortem | "What could go wrong, so that you stop using the program or the idea we are talking about?" |
| Acceptance criterion | Test case: "When this comes in, this should come out" |
| Requirement | "What it has to be able to do" |
| Stakeholder | "Who is affected, and who has to agree?" |
| Scope | "What is part of it, and what is not?" |
| Edge case | Special case |
| Idempotency | "If it runs twice, nothing may happen twice" |
| Rollback | "Back to how it was" |
| Prompt | "Task for Claude to copy" |
| Backlog | "List for later" |
| MVP | "First small version" |
| System, software | "The program", or its name |
| Integration, interface | "Link to [program]" |
| IT | "The people who look after your computers (IT)" |
| Plain text | "Stored in readable form" |
| AI provider | "The company behind this AI" |

## Field names

Field names in this skill are working labels. The user never sees "setting", "care" or "origin" as bare words. Each visible heading is a plain question or phrase. Find the natural one in other languages.

| German | English |
| --- | --- |
| Wo läuft es, wer hat Zugang? | Where does it run, who has access? |
| Wer kümmert sich darum? | Who looks after it? |
| Wer muss zustimmen, bevor ihr es nutzt? | Who has to agree? |
| Woher wissen wir das? (gesagt, angenommen, abgeleitet) | How do we know? (said, assumed, derived) |
| Das soll nicht gebaut werden | Do not build |
| Vorschlag, bitte bestätigen | Suggestion, please confirm |

## Names of the result

| Language | Result | File | Progress file |
| --- | --- | --- | --- |
| German | Bauauftrag | `Bauauftrag.md` | `Zwischenstand.md` |
| English | build brief | `build-brief.md` | `progress.md` |

For other languages, find the natural word. The folder is always called `make-it-go-away/`.

## Fixed phrases

Say these in the user's language. Keep them the same through the whole conversation.

| German | English |
| --- | --- |
| Ergebnis jetzt | result now |
| lass es | leave it |
| noch offen | still open |
| Liste für später | list for later |
| Entwurf | draft |
| Erst klären, dann bauen. | Clarify first, then build. |
| gesagt, angenommen, abgeleitet | said, assumed, derived |
| Reicht dir das, oder machen wir weiter? | Is this enough for you, or shall we go on? |

## Banned

- German: "einfach", "nur", "schnell", when they make the task sound small.
- English: "just", "simply", "quick", "easy", in the same sense.
- The counterparts in every other language.
- Childish tone. Heavy praise: one "good, that helps" is enough.
- Sentences that sound translated word for word.
- Abbreviations nobody explained. Long dashes in running text.

Why these words are banned: they tell the user their problem is small. If it were small, they would not be here.

## When the user speaks the technical language

You notice it when they use two or three technical words correctly.

- Ask once: "You know your way around. Shall I ask more briefly?"
- If yes: shorter questions, fewer examples. Sentences stay short.
- If no, or no answer: carry on as before. Do not ask again.
- Take over the user's own words. If they say "ticket", you say "ticket".
- Never correct a word the user uses. Never lecture.
- If a technical word is used wrongly, ask what they mean in this case. Do not point out the mistake.

## Humour

Friendly, with light humour. At most one wink per stage. Never about errors, law or safety. Never at the user's cost. If in doubt, leave it out.

## Self-check before sending

- Is there exactly one question in this message?
- Is every sentence 15 words or shorter?
- Is there a word my neighbour would not know, or a label from this skill?
- Is there an example answer or a choice?
