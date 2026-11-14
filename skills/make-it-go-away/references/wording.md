# Wording

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

## Field names

These are working labels. The user sees a plain question, never the label.

| German | English |
| --- | --- |
| Wo läuft es, wer hat Zugang? | Where does it run, who has access? |
| Wer kümmert sich darum? | Who looks after it? |
| Wer muss zustimmen, bevor ihr es nutzt? | Who has to agree? |
| Das soll nicht gebaut werden | Do not build |
| Vorschlag, bitte bestätigen | Suggestion, please confirm |

## Fixed phrases

Say these in the user's language and keep them the same all through the conversation.

| German | English |
| --- | --- |
| Ergebnis jetzt | result now |
| lass es | leave it |
| noch offen | still open |
| Liste für später | list for later |
| Entwurf | draft |
| Erst klären, dann bauen. | Clarify first, then build. |
| Reicht dir das, oder machen wir weiter? | Is this enough for you, or shall we go on? |

The result is called "Bauauftrag" in German, with the files `Bauauftrag.md` and `Zwischenstand.md`. In English it is "build brief", `build-brief.md` and `progress.md`. For other languages, find the natural word. The folder is always `make-it-go-away/`.

## Banned

- German "einfach", "nur", "schnell" and English "just", "simply", "quick", "easy", when they make the task sound small. The same in every other language.
- Heavy praise. One "good, that helps" is enough.
- Abbreviations nobody explained. Long dashes in running text.

## Self-check before sending

- Exactly one question in this message?
- Every sentence 15 words or shorter?
- Any word my neighbour would not know, or a label from this skill?
- A choice or example answer, and not one the user can copy as it is?
