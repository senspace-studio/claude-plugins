---
name: updating-records
description: Update the company's records with what actually happened. Write down what someone tells or shows you, and fill in or correct the lists, sheets and trackers people keep by hand from what other records say and from the company's social accounts, such as follower counts and who liked or followed them, writing only what the person approves, where they approve it. Use this whenever someone wants something recorded in the company's records, or wants a list, sheet or tracker brought up to date or checked, such as "Jordan set up the venue today", "here is what they handed me, add it to our records", "add who came to last night's event to the sheet", "update the status column from the meeting notes", "is our member list still right?", or filling a new, empty tracker for the first time.
---

# Update the company's records

Much of what happens is never written down, and what people copy into records by hand contains errors. Values get mistyped, formulas get overwritten, and some values have no source. This skill writes into the company's records what a person tells you, what other records state, and the company's reception. It leaves every decision about a record to the people who keep it.

Three things share the work. The intelligence server searches the company's records, and reports **reception**, meaning the numbers that social platforms such as Instagram report for the company's accounts, like follower counts, and who liked, followed or mentioned those accounts. Its search is refreshed from the records periodically, and does not find anything written after the last refresh. The connector for the service where a record lives reads its current content and writes to it. This skill says how to write.

## What a record holds

A record has parts, entries and fields. In a page, parts are its sections and entries are the items under them, and a page can also carry fields. In a spreadsheet, parts are tabs, entries are rows, and fields are columns. In a database, parts are its tables, entries are their rows, and fields are their columns.

Sort everything in the record into three kinds before writing anything.

- **Structure**: the parts and fields themselves, lists of allowed values, computed parts, settings.
- **Judgment**: what people intend or conclude, such as a target.
- **Facts**: what happened, and what is true now.

People decide structure and judgment. You write facts, and write a judgment only when the person states it. If a fact cannot be written without changing the structure, for example a new column, ask for that change separately from the facts.

Facts come in two kinds.

- **An event** is something that happens, such as someone attending. Each one adds an entry.
- **A state** is one value that changes over time, such as a project's status. Change it only when a source dated after the current value shows a different value. The record's history shows when the current value was written.

If you add a new entry each time a state changes, one thing ends up with several entries. If you record events by overwriting one value, the earlier events are lost.

## Steps

1. **Settle what and where.**
2. **Read the record**, and its reference and settings if it has them.
3. **Gather material** from the person, the records and reception.
4. **Match names** in the material to what the record holds.
5. **Build the changes.**
6. **Show the changes** with their sources, and wait for approval.
7. **Write** what was approved.
8. **Read it back.**

## Settle what and where

A person either tells you something to keep, or names a record to bring up to date.

When they tell you something, find where it belongs. Search the records for what it mentions, and propose either adding to one of those records or creating a new record in the same place as them. Where it goes is part of what they approve. If nothing related turns up, ask where it should go.

When they name a record, settle what to cover, such as which period.

## Read the record

Read the headings, legends and instructions of every part of the record, and find which parts are computed and which ones people fill in.

### References

Read the opening paragraph of each file in `references/`. It says what type of record the file describes and how to recognize one. If the record you are reading is one of them, read the whole reference. A reference describes a type of record that people copy from a template, so many records share its structure, and it says only what the record itself does not show. It opens with what the record is and how to recognize it, then uses these headings:

- **What it is for**: what the computed results measure, and how facts feed them.
- **Parts**: what one entry of each part is, and whether it is structure, judgment, fact, a total or computed.
- **How the parts refer to each other**: which entries name entries in another part, and what the key is.
- **The same fact**: what makes two entries state the same fact.
- **Values and what they mean**: what each value chosen from a list means, and what it makes the totals count.
- **Settings for this skill**: where the record keeps them.

Find where each part lives in the record you are reading. Where the record does not match its reference, report it.

Without a reference, work out the structure from the record itself, and say what you inferred when you show the changes.

### Settings

A record can hold settings for this skill. They say where its related records are kept, such as a folder, and give aliases, the other names that other records use for what this record tracks. A reference says where a type keeps them. If the record has no settings and you need them to narrow a search, propose adding them as a structure change.

## Gather material

### From the person

Keep what they said in their words, and read what they show you.

### From the records

- Search them with intelligence to find where a fact is written, and use the record's settings to narrow the search.
- Search returns a spreadsheet's tab names, row counts and first rows, not the rest of its values. When one looks relevant, open it with its connector and read the values.
- Judge a file by what it holds, not by its title. People file things where it suited them at the time, so a list can sit inside a document named for something else.
- To find records written since the last refresh, such as the notes from this morning's meeting, search with the connector of the service where they live, and read them there.
- The record you are updating can come back from search. It is what you are updating, not a source for it.

### From reception

For facts no record holds, ask intelligence for reception. Each answer holds as of the time it was observed.

## Match names

A name in the material and something the record holds are the same only when a key or an identifier matches exactly, such as an account handle. Treat everything else, such as a first name alone, as a candidate and ask. Create a new entry only after a person confirms that the name matches none of the existing ones.

When search returns a quote saying that two names refer to the same thing, show the quote with the candidate. It helps the person decide. It does not decide for them.

A mistaken match is costly. Where entries refer to each other by key, a duplicate created by mistake cannot be merged later without rewriting every entry that points at it.

## Build the changes

For each fact, decide where it goes, the value, whether it adds an entry or changes a state, and its source. The source of a fact from a record is its title, a link and the passage that states it. The source of a fact from reception is the account, which number or list it is, and when it was observed. The source of a fact the person told you is what they said.

- **Mark your readings.** Text you read off something the person showed you, and dates you worked out, such as from "yesterday", are your readings. Show them as yours until the person confirms them.
- **No source, no value.** A fact you cannot source goes on the "For a person to fill in" list. So does anything you looked for and did not find. If the person then states it, what they said is its source. A record not mentioning something does not mean it did not happen, and someone missing from what reception reports may not have been observed yet.
- **Include what a fact points at.** Where a fact refers to an entry in another record or part that does not exist yet, include that entry in the changes too.
- **One fact, one entry.** Before adding an entry, check whether any entry already states the same fact, including ones people wrote without a source. Processing the same material again must add no new entries.
- **Totals only when stated.** A field that sums up other entries is written only when a record states that number itself or reception reports it. Filling it by counting entries overwrites a number a person counted with one counted a different way.
- **Choose by meaning.** Where a field takes one of a set of values, choose by what each value means, as the reference or the record's legend defines it, not by its label. People rename labels.
- **Do not change or clear a value only because no source supports it.** A person may know it from outside the records, and a record not stating something is not evidence that it is wrong.

## Show the changes

Before writing, show one table of changes. For each change, give where it goes, the value, whether it adds an entry or changes a state, and its source. For example:

| Where | Value | Change | Source |
| --- | --- | --- | --- |
| Page "Spring launch", new entry | 14 May 2026 · Jordan set up the venue | Adds an entry | You said "Jordan set up the venue today" |
| Projects, row "Spring launch", Status | Waiting on venue → Confirmed | Changes a state | [Weekly sync 3 May](link) "Venue signed, launch is on" |
| Contacts, row "@jordanlee", Followers | 640 → 702 | Changes a state | Reception of @studio, follower count of @jordanlee, observed 1 Sep 2026 |

Then list separately:

- Your readings: text you read off what was shown, and dates you worked out.
- Candidates: names you could not match for certain, with the evidence for each possible entry.
- Structure changes you need, and why.
- For a person to fill in: facts with no source, and things you looked for and did not find.
- Anything in the record that looks broken against its own legend or reference. Report it, and do not fix it.

Write only what the person approves. If they approve part, write that part. If they correct a value, write their value, with what they said as its source. The record is theirs. Once it is written, anyone can find it and use it.

## Write

- **Structure first.** Make approved structure changes before writing the facts that need them.
- **Write only where people enter values.** A value written into a computed part either replaces its formula, so every total built on it becomes wrong without any error, or the write is refused.
- **What is pointed at comes first.** Where an entry refers to an entry that is new in this set of changes, write that one first.

## Read it back

Read back what you wrote with the connector. Search does not show it until its next refresh.

- What you wrote is there as you wrote it.
- Every computed part is still computed.
- Every required field in the entries you added is filled.
- The record's own checks pass, if it has any.

Report what you wrote, link to the record, and repeat what still waits on a person: your readings, the candidates, the structure changes, and the "For a person to fill in" list.
