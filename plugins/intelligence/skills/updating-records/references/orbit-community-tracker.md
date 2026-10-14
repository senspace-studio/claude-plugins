# Orbit community tracker

A table for watching how a community changes across its events, based on the Orbit model. Each community keeps its own. You can recognize one by what it tracks: the community's events, its members, a log of what each member did, a list of activity types with weights, and scores called Love, Reach and Gravity that place members in orbits.

## What it is for

The tracker exists to see the community's pull grow from event to event. Its computed scores measure it.

- **Love** is what a person does for the community and how often: taking part, contributing, coming back.
- **Reach** is who a person does it with: their connections inside the community, and their followers outside it.
- **Gravity** combines Love and Reach. Raising it is the goal.
- **Orbits** place each person by distance from the center, the innermost being the core. Each community names its own orbits.
- The center is the community's mission.

A fact feeds the scores through the activity type it is recorded as, the date it carries, and the event it belongs to. Recording someone who helped run an event as merely attending lowers their Love and can put them in the wrong orbit. A wrong date moves when they were last active, and so whether they count as dormant.

## Parts

| Part | One entry is | Kind |
| --- | --- | --- |
| Events | an event the community held | Its name, date, place and kind are facts. Its targets are judgment. Its results, such as attendance, are totals or computed. Check which in the record |
| Members | a person | The name, account, first contact, how they came and their outside followers are facts. The account is the handle that reception reports on. Outside followers is a state, updated from the follower count reception reports for that account. Notes, what they can be asked to do and what can be offered in return are judgment |
| Activity log | one thing a person did | Facts. Each thing a person did is a new entry. Do not record a new activity by changing an existing entry |
| Activity types | a kind of activity | Structure, set up by each community |
| Settings | the tracker's own settings | Structure, set up by each community |
| Scores and dashboards | computed results | Computed |

## How the parts refer to each other

An activity log entry names a member, an activity type and, when it happened at one, an event. The member's name is the key across the whole tracker and must be unique. When two people share a name, add something to the name itself that tells them apart, and let the person choose what to add. Do not change a member's name, since every entry that names the old one would break. If a name looks wrong, report it.

For an entry at an event, leave the date empty, since the tracker uses the event's date. Fill in the date only for an entry with no event. A count on an entry is used only for activity types that count people, such as bringing friends.

## The same fact

Two activity log entries state the same fact when their member, activity type and event are the same. For entries with no event, their dates must also be the same.

## Values and what they mean

Each community sets up its own list of activity types.

The tally tag decides what the totals count. Exactly one activity type carries the tag for attendance. Every person who came to an event gets one entry with it, whatever else they did there. Their other activities at that event are separate entries. The attendance totals and dormancy are computed from those entries, so a missing attendance entry makes a person look as if they never came. If no activity type or more than one carries the attendance tag, report it as broken.

## Settings for this skill

The skill's settings are in the Settings part, next to the tracker's own settings.
