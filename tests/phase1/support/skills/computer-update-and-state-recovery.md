# Computer Update & State Recovery

## When to use
An official update is available, or the client is about to Update, Recover, or Reset the computer. Also use after a rebuild to help restore state.

## Required inputs and access
- Current list of skills
- Key folders under /workspace
- Official docs on what Update / Recover / Reset keep and lose

## Sequence of work
1. Pre-update audit:
   - List the folders currently under /workspace. These are the durable shared area and normally survive an Update.
   - Note that bots, chats, and saved logins are safer still.
   - Flag any installed packages or CLIs that an Update, Recover, or Reset will remove.
   - Note any unsaved work.
   - State a clear boundary line: what is safe vs at risk.
   - Do not move or reorganise any folders.
2. If the client has something critical outside /workspace that they want to keep, tell them the safe options: copy it into a clear folder under /workspace, or copy it to a connected service (Drive, Notion, GitHub for text), or attach the final file to the chat. Do not move anything yourself.
3. Guide the chosen action (Update preferred when available).
4. After the rebuild, check that bots and skills are still present. Offer to re-create any missing skills and reinstall apps as needed. Conversation history and saved bots/files/logins are normally preserved.

## How to validate
The client has a clear list of what is at risk and a plan to protect or restore it. After the action, bots respond and key skills are available.

## What to return
Short audit summary with the boundary line, recommended action, and post-action check list.

## What requires approval
Any Update, Recover, or Reset. Never proceed without explicit client approval.
