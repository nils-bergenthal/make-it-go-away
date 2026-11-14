# Example: lesson reminders in a driving school

This example is invented. All names, firms and numbers are made up. It shows a harder case: personal data of young people, a ready-made tool that may exist, and a verdict of "clarify first".

Lena runs the office of a small driving school. She talks to Claude with the skill switched on.

## The conversation

**Lena:** Make it go away: calling students to remind them of their driving lessons.

**Claude:**

```
This usually takes 10 to 20 minutes. After a few questions I will show you a first draft.
You can say "result now" at any time. This chat runs through the company behind this AI,
so leave out confidential things. Replace names and numbers before you paste anything.
Then show me the last real case.
```

**Lena:** Yesterday I called 11 people. Four did not pick up. Two had forgotten and did not come.

**Claude:**

```
🔹 **Result at the end**

What should be there when this is done?

  a) Every student gets a reminder the day before
  b) Only students who often miss a lesson get one
  c) Something else, describe it briefly
```

**Lena:** a

**Claude:**

```
🔹 **How often**

How many lessons do you remind about, roughly?

  a) About 5 a month
  b) About 50 a month
  c) About 500 a month
```

**Lena:** About 800 a month.

**Claude:**

```
🔹 **Build or not**

At 800 a month, this is worth a look. Your school program may already send
reminders. Nobody has checked yet. What do you want to do?

  a) Check the school program first
  b) Build something of our own
  c) Something else, describe it briefly

**My suggestion:** a), because a ready-made tool would be cheaper and safer.
```

**Lena:** a. I don't know if it can do that.

**Claude:**

```
🔹 **The case that did not fit**

I noted "Does it already exist?" as still open. The company that supplies the program can answer it.

What did the last case look like that did not fit?

  a) A lesson was moved after the reminder
  b) A student did not want any messages
  c) Something else, describe it briefly
```

**Lena:** Both. A moved lesson, and one student who asked us never to send messages.

**Claude:**

```
**Now:** Case. **Next:** Test cases, Risks, Result.
Draft, not final. Goal: every student gets a reminder the day before.
Test case 1: normal lesson. One message the day before.
Test case 2: student wants no messages. No message, stays on your call list.
Still open: does the program already do it, who agreed to messages, where the data goes.

🔹 **Test cases**

I have drafted more cases. Is anything wrong or missing?

  a) The table is right
  b) Something is wrong, I name the row
  c) Something is missing, describe it briefly
```

The table that came with it:

| No. | When this comes in | This should come out |
| --- | --- | --- |
| 1 | Normal lesson tomorrow | One message the day before |
| 2 | Student asked for no messages | No message, stays on the call list |
| 3 | Lesson moved after the message | A new message with the new time |
| 4 | Student has two lessons on one day | One message with both times |
| 5 | No phone number saved | No message, note for Lena |
| 6 | Message cannot be sent | Note for Lena, she calls |
| 7 | Lesson in less than two hours | No message, Lena decides |

**Lena:** Row 7 is wrong. Then we call, always. The rest is right.

**Claude:**

```
🔹 **Where the data lives**

Row 7 is changed. Which programs are involved, and where does the data live?

  a) Everything stays in the school program on our computer
  b) The data leaves the school, for example to a message service
  c) Something else, describe it briefly
```

**Lena:** I don't know. The program is online, I think.

**Claude:**

```
🔹 **Access**

I noted "where the data lives" as still open. The company behind the program can tell you.

Who has access to the lessons and the phone numbers?

  a) Only me
  b) Me and the three driving instructors
  c) Something else, describe it briefly
```

**Lena:** b

**Claude:**

```
🔹 **Looking after it**

Who notices when something is wrong once it runs?

  a) I do
  b) Someone else, I name them
  c) Nobody yet

**My suggestion:** a), with one instructor as stand-in.
```

**Lena:** a

**Claude:**

```
**Now:** Risks. **Done:** Case, Test cases. **Next:** Result.
Still open: who has to agree, whether students agreed to messages.

🔹 **What could go wrong**

What could go wrong, so that you stop using the program or the idea we are talking about?

  a) A message goes to the wrong number
  b) Students complain about messages they did not agree to
  c) Something else, describe it briefly
```

**Lena:** b. Some students do not want that.

**Claude:**

```
🔹 **Is this enough**

Then every student needs a clear yes before the first message. The core is settled.
Is this enough for you, or shall we go on?

  a) Enough, write the result
  b) Go on
```

**Lena:** a

## The result in short form

```
Self-check
Contradictions: none found.
Assumptions: rows 4 and 6 are my suggestion.
Gaps: does the program already do it, where the data goes, who agreed, how long data is kept.
```

**Build brief (short form)**

> **Verdict: clarify first.** Reminders are worth having at 800 a month, but two answers could change everything.
> For the boss, in one sentence: Probably yes, but not before we know if the program can already do it and if students agreed to messages.
> Conditions before building: 1. The company behind the program says if reminders exist. 2. Someone checks that students agreed to messages.
> Personal data of students is involved, some of them under 18. This is a reminder to check, not legal advice.

| Field | Content |
| --- | --- |
| Goal | Every student who agreed gets a reminder the day before |
| How often | About 800 a month |
| Where does it run, who has access? | Practice program, online. Access for Lena and three driving instructors. Where the data goes: still open. |
| Test cases | The seven rows above, row 7 changed to "Lena calls" |
| Special cases | Moved lessons, two lessons a day, no number |
| Risk | Messages to students who did not agree. Countermeasure: only students with a saved yes get one. This is my suggestion. |
| Who has to agree? | Still open: the person for data protection. |
| Who looks after it? | Lena |
| List for later | Replies from students |

**Task for Claude to copy (short form)**

- At the top: the condition "Does the program already do it?" and the open question who has to agree.
- Goal, programs and access as in the build brief.
- The seven test cases.
- Limits: no message to students without a yes. Lena calls when a lesson is less than two hours away.
- Do not build: answering replies from students.
- Data protection paragraph: Which data: name, phone number, lesson time. Some students are under 18, so treat the data with extra care. Who may see it: Lena and the three driving instructors. How long it is kept: still open. Where it stays: still open. This is a reminder to check, not legal advice.

**Suggestion, please confirm (not part of the task)**

- No details about fees or test results in any message.
- A test week with five students who agreed.

**Final recommendation**

Have it checked first. Personal data of young people and many students are involved. Before building, have the brief checked by a second place, for example the person for data protection.

Next step: Lena asks the company behind the program if reminders exist.
