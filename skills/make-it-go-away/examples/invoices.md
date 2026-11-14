# Example: invoices from emails into a table

This example is invented. All names, firms and numbers are made up. It shows the layout, the length and the tone.

Mara runs the office of a small joinery. She talks to Claude with the skill switched on.

## The conversation

**Mara:** Make it go away: typing invoices from emails into our table.

**Claude:**

```
This usually takes 10 to 20 minutes. After a few questions I will show you a first draft.
You can say "result now" at any time. This chat runs through the company behind this AI,
so leave out confidential things. Replace names and numbers before you paste anything.
Then show me the last real case.
```

**Mara:** Yesterday a wood supplier mailed a PDF invoice. I typed date, supplier, invoice number and amount into the table. Then I moved the PDF into a folder.

**Claude:**

```
◉ Result at the end

What should be there when this is done?

  a) Every invoice is a row in the table
  b) Every invoice is a row, and unpaid ones stand out
  c) Something else, describe it briefly
```

**Mara:** b

**Claude:**

```
◉ How often

How often does this happen, roughly?

  a) About 5 times a month
  b) About 50 times a month
  c) About 500 times a month
```

**Mara:** About 60.

**Claude:**

```
◉ Build or not

At 60 a month, I would build it, and you check the first results.
The other way is a ready-made tool. Which do you prefer?

  a) Build it
  b) Look for a ready-made tool first
  c) Something else, describe it briefly

My suggestion: a), because 60 a month is a lot of typing.
```

**Mara:** Build it. We pay for enough tools already.

**Claude:**

```
◉ The case that did not fit

What did the last case look like that did not fit?

  a) An email with more than one invoice
  b) Something that looked like an invoice and was not
  c) Something else, describe it briefly
```

**Mara:** A paint shop sent one email with two invoices. I missed the second one. And once a reminder looked like an invoice.

**Claude:**

```
Now: Case. Next: Test cases, Risks, Result.
Draft, not final. Goal: every invoice from the mailbox is a row in the table.
Test case 1: one email, one PDF invoice. One new row, PDF filed.
Test case 2: one email, two PDF invoices. Two new rows.
Still open: how paying is handled, where the table lives, who looks after it.

◉ Test cases

I have drafted more cases. Is anything wrong or missing?

  a) The table is right
  b) Something is wrong, I name the row
  c) Something is missing, describe it briefly
```

The table that came with it:

| No. | When this comes in | This should come out |
| --- | --- | --- |
| 1 | Email with one PDF invoice | One new row, PDF filed |
| 2 | Email with two PDF invoices | Two new rows |
| 3 | Reminder for an old invoice | No new row, note for Mara |
| 4 | Credit note | Mara decides |
| 5 | Same invoice sent twice | One row, not two |
| 6 | PDF that cannot be read | No row, message to Mara |

**Mara:** Row 4 is wrong. A credit note goes in with a minus. Oh, and could it pay the invoices too?

**Claude:**

```
◉ Paying later

I put "paying invoices" on the list for later. Row 4 is changed.

Which programs are involved, and where does the data live?

  a) Email program and a table on a shared drive
  b) Email program and an online table
  c) Something else, describe it briefly
```

**Mara:** Outlook with a shared mailbox. The Excel file is on the shared drive.

**Claude:**

```
◉ Access

Who has access to the mailbox and the file?

  a) Only me
  b) A few people in the office
  c) Something else, describe it briefly
```

**Mara:** My boss Jonas and I.

**Claude:**

```
◉ Looking after it

Who notices when something is wrong once it runs?

  a) I do
  b) Someone else, I name them
  c) Nobody yet

My suggestion: a), with Jonas as stand-in.
```

**Mara:** I don't know. Probably me.

**Claude:**

```
Now: Risks. Done: Case, Test cases. Next: Result.
Still open: who looks after it, who has to agree.

◉ What could go wrong

What could go wrong, so that you stop using the program or the idea we are talking about?

  a) Access to the mailbox runs out
  b) Suppliers change their invoice layout
  c) Something else, describe it briefly
```

**Mara:** b. Suppliers change theirs all the time.

**Claude:**

```
◉ Is this enough

Then an unclear invoice goes to you and not into the table. The core is settled.
Is this enough for you, or shall we go on?

  a) Enough, write the result
  b) Go on
```

**Mara:** a

## The result in short form

```
Self-check
Contradictions: none found.
Assumptions: that unpaid invoices get their own column is my suggestion.
Gaps: who looks after it, how long PDFs are kept, who has to agree.
```

**Build brief (short form)**

> **Verdict: build with conditions.** Typing 60 invoices a month is worth automating, and the rules are clear.
> For the boss, in one sentence: Yes, this is probably worth it, because it saves a lot of typing, but someone must be named who looks after it.
> Conditions before building: Jonas says who looks after it. Someone from bookkeeping looks once at the table layout.
> **Stop notice:** Clarify first, then build. Missing: who looks after it.

| Field | Content |
| --- | --- |
| Goal | Every invoice from the mailbox is a row in the table. The PDF is filed. Unpaid ones stand out. |
| How often | About 60 a month |
| Where does it run, who has access? | Outlook shared mailbox, Excel file on the shared drive, access for Mara and Jonas |
| Test cases | The six rows above, row 4 with a minus |
| Special cases | Two invoices in one email, reminders, credit notes |
| Risk | Suppliers change their layout. Countermeasure: unclear invoices go to Mara. |
| Risk | Access to the mailbox runs out. Countermeasure: a message to Mara after one day without a run. This is my suggestion. |
| Who has to agree? | Still open. |
| Who looks after it? | Probably Mara. Jonas decides. Still open. |
| List for later | Paying invoices |

**Task for Claude to copy (short form)**

- At the top: the stop notice, and the open question who has to agree.
- Goal, programs and access as in the build brief.
- The six test cases.
- Limits: unclear invoices go to Mara. The same invoice is entered once.
- Do not build: paying invoices.
- Marked as my suggestion: the message after one day without a run.

**Suggestion, please confirm (not part of the task)**

- No changes to old rows.
- No deleting of emails.

**Final recommendation**

Build once Jonas has said who looks after it. Because the numbers feed the bookkeeping, have someone from bookkeeping look at the table layout once before you start. This is a reminder to check, not tax advice.

Next step: Mara asks Jonas who looks after it, then hands over the task.
