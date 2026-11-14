# Example: invoices from emails into a table

This example is invented. All names, firms and numbers are made up.

Mara runs the office of a small joinery. She talks to Claude with the skill switched on.

## The conversation

**Mara:** Make this go away: typing invoices from emails into our table.

**Claude:** This usually takes 10 to 20 minutes. After a few questions I will show you a first draft. You can say "result now" at any time. This chat runs through the company behind this AI. Replace names and numbers before you paste anything. Then show me the last real case.

**Mara:** Yesterday a wood supplier sent an email with a PDF invoice. I typed date, supplier, invoice number and amount into the table. Then I moved the PDF into a folder.

**Claude:** Thanks, that is clear. Which result should be there at the end? For example: "Every invoice is a row in the table, and the PDF is filed."

**Mara:** Yes, that. And I want to see which ones are not paid yet.

**Claude:** Noted. How often does this happen, roughly? 5, 50 or 500 times a month?

**Mara:** About 60.

**Claude:** At 60 a month, I would build it, with you checking at first. A ready-made tool is the other option. Which do you prefer?

**Mara:** Build it. We pay for enough tools already.

**Claude:** Fair. What did the last case look like that did not fit?

**Mara:** A paint shop sent one email with two invoices. I missed the second one. And once a reminder looked like an invoice.

**Claude:** Here is a first draft.

- Goal: every invoice from the mailbox is a row in the table.
- Test case 1: one email, one PDF invoice. One new row, PDF filed.
- Test case 2: one email, two PDF invoices. Two new rows.
- Still open: where the table lives, who looks after it.

Is this enough for you, or shall we go on?

**Mara:** We go on. Oh, and could it pay the invoices too?

**Claude:** I put "paying invoices" on the list for later. Here are the test cases. Is anything wrong or missing?

| No. | When this comes in | This should come out |
| --- | --- | --- |
| 1 | Email with one PDF invoice | One new row, PDF filed |
| 2 | Email with two PDF invoices | Two new rows |
| 3 | Reminder for an old invoice | No new row, note for Mara |
| 4 | Credit note | Mara decides |
| 5 | Same invoice sent twice | One row, not two |
| 6 | PDF that cannot be read | No row, message to Mara |

**Mara:** Row 4 is wrong. A credit note goes in with a minus.

**Claude:** Changed. Which programs are involved, and where does the data live? Example: "Outlook, an Excel file on the shared drive, three people have access."

**Mara:** Outlook with a shared mailbox. The Excel file is on the shared drive. My boss Jonas and I have access.

**Claude:** Who looks after it once it runs? Example: "Me, and Jonas when I am away."

**Mara:** I don't know. Probably me.

**Claude:** I note that as still open. Jonas could decide it. What could go wrong, so that you stop using the program or the idea we are talking about? My three guesses: mailbox access expired, a new invoice layout, nobody felt in charge. Which one fits best?

**Mara:** The layout. Suppliers change theirs all the time.

**Claude:** Then an unclear invoice goes to you and not into the table. The main points are settled now. Shall I write the result?

**Mara:** Yes, result now.

## The result in short form

**Self-check**

- Contradictions: none found.
- Assumptions: unpaid invoices get their own column. Jonas has to agree.
- Gaps: who looks after it, how long PDFs are kept, other approvals (not asked).

**Build brief (short form)**

| Field | Content | How do we know? |
| --- | --- | --- |
| Goal | Every invoice from the mailbox is a row in the table. The PDF is filed. | said |
| How often | About 60 a month | said |
| Where does it run, who has access? | Outlook shared mailbox, Excel file on the shared drive, access for Mara and Jonas | said |
| Test cases | The six rows above, row 4 with a minus | derived, confirmed |
| Special cases | Two invoices in one email, reminders, credit notes | said |
| Risk | New invoice layout. Countermeasure: unclear invoices go to Mara. | said |
| Risk | Mailbox access expires. Countermeasure: a message to Mara after one day without a run. | assumed |
| Who has to agree? | Jonas, as the boss. Still open. | assumed |
| Who looks after it? | **Stop notice: Clarify first, then build.** Probably Mara. Jonas decides. | still open |
| List for later | Paying invoices | said |

**Task for Claude to copy (short form)**

- At the top: the stop notice and the open approval by Jonas.
- Goal, programs and access as in the build brief.
- The six test cases.
- Limits: unclear invoices go to Mara. The same invoice is entered once.
- Do not build: paying invoices.
- Marked "(assumed)": the message after one day without a run, the yes from Jonas.

**Suggestion, please confirm (not part of the task)**

- No changes to old rows.
- No deleting of emails.

**Final recommendation**

Build once Jonas has said who looks after it. Little is at stake here, so no second check is needed.

Next step: Mara asks Jonas who looks after it, then hands over the task.
