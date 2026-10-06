---
name: update-from-records
description: Bring a table that people keep by hand up to date from the company's records, with a source for every value and nothing written until a person approves. The table can be a spreadsheet or a database of events, attendees, members, contacts, projects or statuses. Use this whenever someone wants such a table filled in, caught up or checked against what actually happened, even if they never say "table" or "records", such as "add who came to last night's event to the sheet", "update the status column from the meeting notes", "is our member list still right?", or filling a new, empty tracker for the first time.
---

# Update a table from the records

People copy facts out of the company's records into tables they keep by hand. Copying by hand drifts. Values get mistyped, formulas get overwritten, and values that no record supports creep in. This skill writes into such a table the facts the records state, each with its source, and leaves every decision about the table to the people who keep it.

Three things share the work. Intelligence finds where a fact is written and returns numbers about the company's accounts. The connector for wherever the table lives reads and writes its values. This skill holds how to write into the table.

## What the table holds

A table is made of parts, entries and fields: in a spreadsheet, tabs, rows and columns; in a database, the databases, their pages and properties. This skill says rows and columns for both.

Sort everything in the table into three kinds before writing anything.

- **Structure**: tabs or databases, headers, legends, lists of allowed values, computed columns, settings.
- **Judgment**: targets, assessments, notes, plans.
- **Facts**: what happened, and what currently holds.

People decide structure and judgment. You write facts. If a fact cannot be written without changing the structure, for example a new column, tab or property, ask for that change separately from the facts.

Facts come in two kinds.

- **An event** happens and adds one more. Add a row for it.
- **A state** is one value that moves over time. Change it only when a record newer than the current value states the change.

Adding a state as rows stacks up copies of one thing. Overwriting an event as a state erases the ones before it.

## Steps

1. **Read the table**, with its reference and settings.
2. **Settle the scope**: which period, events, people or projects to cover.
3. **Gather material** from the records.
4. **Match names** in the records to rows in the table.
5. **Build the changes.**
6. **Show the changes** and wait for approval.
7. **Write** what was approved.
8. **Check** the table after writing.

## Reading the table

Read the headers, legends and instructions of every part of the table, and find which columns are computed and which ones people fill in.

### References

Read the opening paragraph of each file in `references/`. It says what type of table the file describes and how to recognize one. If the table you are reading is one of them, read the whole reference. A reference describes one type of table that people copy, and only what the table itself does not show. It opens with what the table is and how to recognize it, then uses these headings:

- **What it is for**: what the computed results measure, and how facts feed them.
- **Parts**: what one entry of each part is, and whether it is fact, judgment, a total or computed.
- **How the parts refer to each other**: which entries name entries in another part, and what the key is.
- **The same fact**: what makes two entries state the same fact.
- **Values and what they mean**: what each value chosen from a list means, and what it makes the totals count.
- **Settings for this skill**: where the table keeps them.

A reference describes the type, not any one copy. Find where each part lives in the table you are reading. Where the table does not match its reference, report it.

Without a reference, work out the structure from the table itself, and say what you inferred when you show the changes.

### Settings

A table can hold settings for this skill: where its records are kept, such as accounts and folders, and other names the records use for the things it tracks. A reference says where a type keeps them. If a table has none and the search needs them, ask to add them, as a structure change.

## Gathering material

- Search the records with intelligence to find where a fact is written. Use the table's settings to aim the search.
- Search returns a spreadsheet as what it holds, not its values. When one looks relevant, open it with its connector and read the values.
- Judge a file by what it holds, not by its title. People file things where it suited them at the time, so a list can sit inside a document named for something else.

## Matching names

A name in a record and a row in the table are the same only when a key or an identifier matches exactly, such as the table's key column, an account handle or an ID. Treat everything else as a candidate and ask, including similar spellings, first names alone and nicknames. Create a new row only after a person confirms that the name matches none of the existing rows.

When intelligence returns a connection between two names, show its quote with the candidate. It helps the person decide. It does not decide for them.

A mistaken match is costly. Where rows refer to each other by key, a duplicate created by mistake cannot be merged later without rewriting every row that points at it.

## Building the changes

For each fact, decide where it goes, the value, whether it adds a row or changes a state, and its source: the record's title, a link, and the passage that states it.

- **No source, no value.** A fact you cannot source goes on the list for a person. So does anything you looked for and did not find. A record not mentioning something does not mean it did not happen.
- **Include what a fact points at.** Where a fact refers to a row in another table or tab that does not exist yet, include that row in the changes too.
- **One fact, one row.** Before adding a row, check whether any row already states the same fact, including rows people wrote without a source. Running this again must not add anything.
- **Totals only when stated.** A field that sums up other rows is written only when a record states that number itself. Filling it by counting rows overwrites a number a person counted with one counted a different way.
- **Choose by meaning.** Where a column takes one of a set of values, choose by what each value means, as the reference or the table's legend defines it, not by its label. People rename labels.
- **Leave values only the table holds as they are.** A person may know them from outside the records, and a record not stating something is not evidence that it is wrong.

## Showing the changes

Before writing, show one table of changes. For each change, give where it goes, the value, whether it adds a row or changes a state, and its source with the quoted passage. For example:

| Where | Value | Change | Source |
| --- | --- | --- | --- |
| Attendance, new row | Event 12 · Jordan Lee · attended | Adds a row | "Event 12 guest list", link: "Jordan Lee — checked in" |
| Projects, row "Spring launch", Status | Waiting on venue → Confirmed | Changes a state | "Weekly sync 3 May", link: "Venue signed, launch is on" |

Then list separately:

- Candidates: names you could not match for certain, with the evidence for each possible row.
- Structure changes you need, and why.
- For a person to fill in: facts with no source, and things you looked for and did not find.
- Anything in the table that looks broken against its own legend or reference. Report it, and do not fix it.

Write only what the person approves. If they approve part, write that part. The table is theirs, and they are the ones who will answer for what it says.

## Writing

- **Write only where people enter values.** A value written into a computed column either replaces how it is computed, so every total built on it goes quietly wrong, or is refused.
- **What is pointed at comes first.** Where a row refers to a row in another table or tab that is new in this set of changes, write that row first.
- **Every value carries its source.** Attach it as a note or comment on the value, unless the reference names another place. Without a source, nobody can later tell whether the value still holds.

## After writing

- Every computed column is still computed.
- Every required field in the rows you added is filled.
- The table's own checks pass, if it has any.

Report what you wrote, link to the table, and repeat the lists that still need a person.
