# Orbit community tracker

A table for watching how a community changes across its events, based on the Orbit model. Each community keeps its own. You can recognize one by what it tracks: the community's events, its members, a log of what each member did, a list of activity types with weights, and scores called Love, Reach and Gravity that place members in orbits.

## What it is for

The tracker exists to see the community's pull grow from event to event. Its computed scores measure it.

- **Love** is what a person does for the community and how often: taking part, contributing, coming back. It is computed from the person's activities, each weighted by how much it means and faded over time, together with how many distinct days they were present and how many kinds of channel they were active in.
- **Reach** is who a person does it with: their connections inside the community, and their followers outside it.
- **Gravity** is Love × Reach, the community's total pull. Raising it is the goal.
- **Orbits** place each person by distance from the centre, the innermost being the core. Each community names its own orbits.
- The centre is the community's mission.

The scores are only for comparing people with each other, and a time with an earlier time. Their absolute values mean nothing.

A fact feeds the scores through the activity type it is recorded as, the date it carries, and the event it belongs to. Recording someone who helped run an event as merely attending lowers their Love and can put them in the wrong orbit. A wrong date moves when they were last active, and so whether they count as dormant.

## Parts

| Part | One entry is | Kind |
| --- | --- | --- |
| Events | an event the community held | Its name, date, place and kind are facts. Its targets are judgment. Its results, such as applications and attendance, are totals |
| Members | a person | The name, account, first contact, how they came and their outside followers are facts. Notes, what they can be asked to do and what can be offered in return are judgment |
| Activity log | one thing a person did | Facts. Each entry is an event in the sense of the skill: add entries |
| Activity types | a kind of activity, with its weight, stage, channel and tally tag | Set up by each community |
| Settings | the mission, orbit names, model parameters, the focus event | Set up by each community |
| Scores and dashboards | computed results | Computed |

## How the parts refer to each other

An activity log entry names a member, an activity type and, when it happened at one, an event. The member's name is the key across the whole tracker and must be unique. People with the same name are told apart within the name. Renaming a member breaks every entry that names the old one.

An entry without a date takes its event's date. Give an entry its own date only when it happened outside an event. A count on an entry is used only for activity types that count people, such as bringing friends.

## The same fact

Two activity log entries state the same fact when their member, activity type and event are the same.

## Values and what they mean

Each community sets up its own list of activity types, so choose one by what it means: its description, its stage, its channel and its tally tag.

The tally tag decides what the totals count. Exactly one activity type carries the tag for attendance. Every person who came to an event gets one entry with it. Attendance counts, repeat rates, first-time flags and dormancy are all computed from those entries, so a missing attendance entry makes a person look as if they never came. Other tags drive the totals for friends brought and people who helped.

## Settings for this skill

Keep the skill's settings with the tracker's own settings.
