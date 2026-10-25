# EA Setup Skill

## When to use
When creating or updating a specialist bot, or when setting house rules for this account.

## Required inputs and access
Client profile answers (business, timezone, size, time sinks, one 7-day win, actual tools they use).

## Sequence of work
1. Fetch the pack manifest from its public raw URL. Record the required bots and completion rule.
2. Confirm the profiling answers are recorded, including the real tool list.
3. For each required specialist in order: fetch its template.yaml, state exact job, approval_never list, first_task, and proposed early routine. Tell it which tools the client actually has.
4. Create the bot (or instruct the user to create it) and paste the generated Description.
5. Confirm the needed connections for the client’s actual tools.
6. Ask the specialist to run its first_task and produce one sample.
7. After each bot (and whenever the user returns), re-check the manifest. If any required bot is still missing, re-prompt to finish it before other work.
8. When the pack is complete, summarise what was created and any remaining human decisions.

## How to validate
Specialist exists with narrow job and explicit never-do list. Sample output matches its deliverable format. No messages sent. It is using the client’s real tools, not a hard-coded stack.

## What to return
Short creation summary + sample output from the specialist.

## What requires approval
Creating additional specialists beyond the agreed first one. Any change that expands scope or removes an approval gate.
