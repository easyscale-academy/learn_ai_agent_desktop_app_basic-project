---
description: "You have picked this teaching repo as your working folder in Claude Code Desktop, walked through every action against twenty-four screenshots, had the AI write a doc from those screenshots, generated a summary with the summarize skill, checked what is eating your context window, and successfully forked a new session that only inherits part of the history."
---

# Walk Through the Full Claude Code Desktop Workflow

## 1. Goal

Walk the entire path of Claude Code Desktop by hand: from picking a folder to actually putting an Agent Skill to work. The goal isn't to memorize every button's name — it's to turn this app from "a screen full of things I don't recognize" into "I know what every part of this does."

By the end you'll have two real deliverables sitting in your own repo: a doc the AI wrote based on screenshots, and a long-form summary produced by an Agent Skill.

---

## 2. What to do

1. Clone this teaching repo locally. Open the Claude desktop client and switch from Home to Code in the top left.
2. Click the folder button, use Open folder to pick the folder you just cloned, and send a first message to confirm the connection works.
3. Click through these seven spots one by one: Local, main and worktree, the add-folder button, the permission mode, the plus menu, Model, and Effort. Set the permission mode to Auto.
4. Take a screenshot of the Claude Code interface itself, paste it into the input box, and have it write a doc based on that screenshot into some markdown file under the tmp directory. Once it's done, click the file link in the chat log to see the rendered result, then use the three-dot vertical menu to open Files and locate it in the file tree.
5. Read the doc it wrote. Pick a spot where it doesn't match what you're actually seeing on screen, take another screenshot, follow up about it, and have it search the web — watch how it corrects itself.
6. In the file tree, find claude-agent-skills.md under the resources directory, right-click it and choose Attach as context. Type a slash followed by "summari", press Tab to autocomplete, send it, and watch the structure of the output.
7. Type a slash followed by "context" and read that breakdown table from top to bottom, paying special attention to how much the Messages row takes up and the total used.
8. Pick any message in the middle of the conversation, click Fork from here, and confirm the new session only inherits the history up to that branch point.

**Estimated time:** 60 to 90 minutes

---

## 3. Checklist

- [ ] **Working folder selected**: you switched from Home to Code, selected your local repo folder, and got a reply to your first message.
- [ ] **You know every widget**: you clicked through Local, main and worktree, add-folder, permission mode, the plus menu, Model, and Effort, and you can explain what each one does.
- [ ] **Weighing permission modes**: you can explain why Auto is the everyday default, when it's worth switching to Plan mode first, and why Bypass permissions is only for people who can absorb the risk of it themselves.
- [ ] **Judging Effort**: you can name at least two kinds of tasks and say whether each should lean toward the Faster end or the Smarter end, and explain why higher isn't always better.
- [ ] **Handing over materials and writing files**: you handed over material via a screenshot, had the AI write output to a path you specified, and you know the tmp directory is a gitignored scratch area.
- [ ] **Screenshot-and-ask as a method**: you handed the AI a screenshot of the interface and asked about it at least once, followed up on one mismatch by asking it to search the web, and you agree this is the most direct way to get up to speed on any unfamiliar piece of software.
- [ ] **Reviewing changes**: you clicked a file link in the chat log to see the rendered result, and also browsed the file tree using the Files panel.
- [ ] **Used an Agent Skill**: you successfully invoked the summarize skill and got a summary back, and you can point to the skill's actual source, the SKILL.md file for summarize under the skills folder inside .claude.
- [ ] **Seeing through the context window**: you ran the context command, can say how much the Messages row takes up versus the total used, and can name at least three things that occupy context but never show up in the chat log (the system prompt, tool descriptions, the skill manifest, the full text of files you've read, intermediate steps).
- [ ] **Fork worked**: you forked a new session and confirmed it only inherited the history up to the branch point.
