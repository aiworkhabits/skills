---
name: done
description: Wrap up a finished task. Checks the result against what the user originally asked for, lists anything still missing, then cleans up after this chat, saves what's worth remembering, and asks whether to archive the chat. Use when the user says "/done", "$done", "done", "wrap up", "we're finished", or "close this out". Don't use it for quick questions.
---

# Done

Work only on this chat and the folder it is running in. Write in the language the user has been using. Keep it short and plain, because the user may not be technical.

## Safety rules

- Never delete, move or overwrite anything this chat didn't create. List it and ask first.
- Before deleting anything this chat did create, show the list and wait for a yes.
- Never publish, push, send, or share anything as part of wrapping up.
- Never write passwords, keys or verification codes into any file.

## Step 1: Check the work

1. Find what the user actually asked for in this chat. Use their own words, plus any change they agreed to later. If there were several tasks, list each one.
2. Check every item now. Open the file, load the page, run the test, count the rows. Don't go from memory.
3. Give proof for each item: a file path, a link, a number, a test result or a screenshot. If you can't prove it, write "not verified". Don't write "should be fine".
4. If anything is still running in the background, the task isn't done. Wait for it, then check what it produced yourself.

## Step 2: If something is missing, stop here

- If it's inside what the user already asked for and you can do it, finish it and go back to Step 1.
- If not, show two short lists and stop. Don't clean up and don't archive.
  - **Still missing:** what it is, where it falls short, what's blocking it.
  - **Needs you:** sign-ins, codes, payments, decisions. Say exactly where to click and what they'll see.

## Step 3: If everything is done, tidy up

Skip any line that doesn't apply.

1. **Leftovers.** List the temporary files, test scripts and replaced drafts this chat created. Delete them only after the user says yes. If there's any doubt, move the file into an `archive` folder in this project, and never overwrite a file that's already there.
2. **Files in the right place.** Final files stay where the project keeps them. Working notes from finished work go into `archive`.
3. **Project instructions.** If this chat changed how things are done, show what you'd change in the project's instruction file (`CLAUDE.md` or `AGENTS.md`) and make the change after the user says yes. Never touch global instructions unless the user asks.
4. **Memory.** If this tool keeps memory or the project has a notes file, save only what the user decided or what was proven to work. One fact per entry, with the reason. Update an old entry instead of adding a duplicate. If there's no place for memory, offer a short note the user can keep.
5. **What's next.** If there's more to do later, write down the next step and the decisions already made, so a new chat can pick it up.

## Step 4: Report and ask

Fit it on one screen:

- **Result:** done, or how many items are left.
- **Proof:** each thing the user asked for, next to its proof.
- **Changed:** what you cleaned up, moved or saved.
- **Not verified:** anything you couldn't check. Write "none" if there's nothing.
- **Next:** the next step, or "none".

Then ask: "Archive this chat, or keep it open?"

- If they choose archive and this app gives you a way to archive the chat, do it.
- If it doesn't, say so and tell the user they can archive it themselves.
- Never delete the chat.
