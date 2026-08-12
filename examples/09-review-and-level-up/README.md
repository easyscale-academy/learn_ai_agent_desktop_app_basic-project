---
description: "By the end you can name the eight things Claude Code, Codex, and Antigravity all share as Agent Apps, know that this course deliberately stops at 'enough to work with' and which directions to push in if you want more, and see how the boss mindset from Task 08 fits together with these shared traits into one complete picture."
---

# Review and Level Up, You Basically Know How to Use an AI Agent Now

> This is the last piece in the course. It doesn't teach anything new; it does one thing: take everything from the earlier pieces and reassemble it into one picture you can carry with you.

## 1. A Few Words to Open the Last Piece

By now you've gotten comfortable with at least one of [Claude Code](../05-claude-code/README.md) or [Codex](../06-codex/README.md) (the Antigravity piece isn't open yet, see the note in [Task 07](../07-antigravity/README.md)), and you've practiced using it faster in [Task 08](../08-plan-and-delegate/README.md). This piece doesn't teach any new buttons. It does three things: pull out what these tools have in common, so switching to any new one later doesn't mean starting from scratch; say plainly where this course stops and where to go if you want to push further; and bring Task 08's mindset back to close things out.

---

## 2. Stake Out Your Territory First, Bind a Folder and a GitHub Repo

Whether it's Claude Code, Codex, or Antigravity, the first move at the start of any job is always the same: give it a piece of territory. That territory is a local folder, and it usually maps to a GitHub repo too. Without that territory, the Agent has nowhere to start — it can't read your stuff, and it has nowhere to write.

[Task 02](../02-why-learn-this/README.md) put it as "one task equals one folder, and that folder is a repo," and you picked that territory yourself back in Tasks 05 and 06. This isn't a feature of any single tool — it's the common starting point for every Agent App of this kind.

---

## 3. Use the File Explorer to See What's in Your Territory

Once the folder is bound, all three tools come with a **file explorer** so you can always see what's currently in that territory and which files the Agent just changed. It's not decoration — it's the main thing that lets you trust what the Agent tells you it did. When it says it's finished, you open the file explorer, take a look, and you know whether it actually did the work, and whether it did it right.

---

## 4. Read and Write Files, Including Images

With the territory staked out and the explorer in hand, what's left is the actual work. All three tools can **read and write files**, and they can also **read and write images**: you can hand it a screenshot and have it understand what's on screen, or have it read a document and edit it, write it, or reorganize it into a new file for you. This is the most basic capability that makes them Agents rather than just chatbots — the formula from [Task 03](../03-model-chatbot-agent/README.md), base model plus harness, shows up here in concrete form.

---

## 5. Permission Mode, Deciding Whether It Asks Before Acting

The three things above are about what it can do. This one is about whether it asks you first.

All three tools have this switch, they just call it different things: in Claude Code it's the **permission mode**, in Codex it's the **approval mode**. The number of settings differs too, but they're arranged along the same axis: from "ask me before every single step," to "use your own judgment and only ask about potentially unsafe actions," to "full access, stop asking." You already set it once back in Task 05 or Task 06, and both pieces called it the single most important switch — that wasn't an exaggeration.

Why does it matter? Because the biggest difference between an Agent and a ChatBot is that an Agent actually touches your stuff. If it can touch, it can touch the wrong thing. This switch decides how much freedom you hand over at once.

The middle setting is the comfortable one for daily work: too strict and you get pestered constantly, wide open and you'd better be able to absorb your own losses. And one rule of thumb holds across all three tools: **the looser you set permissions, the more you should be using branches as your undo mechanism** — the two go together.

---

## 6. Session, Chat, Context, the Same Memory Model

All three tools organize your interaction with them the same way: a **session** is a conversation built around a particular goal, a session is made up of round after round of **chat**, and all of that conversation, plus every file it has read, adds up to the **context** it's currently holding in its head.

This model isn't a coincidence — every Agent App has to solve the same problem: how does the AI remember where this task started and how far it's gotten. [Task 08](../08-plan-and-delegate/README.md) taught you to write planning documents, and at bottom that's an insurance policy against this memory model: context can get lost, but files don't.

---

## 7. Adjust the Model and Effort Level, Like Shifting Gears

All three tools let you pick a **model**, and they all let you tune **Effort** (how hard it thinks). It's like shifting gears in a car: for simple, straightforward work, a cheap, fast gear is enough; for complex work that needs real thought, shift to a smarter gear that's willing to put in more work — slower and pricier, but worth it. Task 03 explained that what you're paying for is compute, and the model and Effort choices here are the actual dial in your hand for deciding where that money goes.

---

## 8. Agent Skill, One Standard Shared Across the Whole Industry

All three tools support **Agent Skill**, and this isn't something each vendor invented separately — it's **one standard shared across the whole industry**. Once you learn how to use a Skill in Claude Code, the way you use one in Codex or Antigravity barely changes — at most the button is in a different spot. In Tasks 05 and 06 you used a bare-bones summarize skill with your own hands, and that's the most basic use of this standard: taking a way of working you do over and over and writing it up as instructions the Agent can follow.

---

## 9. Fork, Starting Fresh from a Fork in the Road

All three tools have a **Fork** feature: branch off from some point in the conversation into a new line, without touching the original one. This is especially handy when you want to "try a different approach, but don't want to lose the progress the current path has already made" — it's the same idea as branching in Git, except what you're branching is the conversation, not the code.

---

## 10. If You Want to Go Further, Where to Go

Let's be straight about one thing: this course stops at "enough to work with."

What you have in your hands right now is already enough to hand off most of your daily reading, looking things up, writing, and organizing — more than enough to get real work done. But honestly, this course probably covers less than twenty percent of what these apps can actually do. The other eighty percent isn't beyond you; it's deliberately left out. Grabbing at everything while you're still getting started only leaves you shaky at all of it.

So this section teaches nothing. It just gives you three directions and the door into each, so you know where to start when you're ready to push further.

**Direction one, and the most important: learn to read the official docs yourself, with an AI beside you.**

All three vendors write detailed official documentation, and it's the only source that keeps up with the versions. Second-hand tutorials, videos, and posts are mostly somebody else's chewed-over take, and they're usually already out of date (this course included — you saw the screenshots not matching your real interface back in Tasks 05 and 06). Reading the source used to be a high bar. It isn't anymore: you have an Agent that will walk through it with you paragraph by paragraph.

- Search terms: `Claude Code documentation`, `OpenAI Codex documentation`, `Antigravity documentation`
- One-line prompt: "This is a page from the official docs. Walk me through it section by section as if I have no programming background, and tell me which parts I can use right now and which parts I can skip for later."

**Direction two: the professional user's own backyard.**

Pairing it with professional dev tools and programming languages, pairing it with the terminal, having the AI automate a browser to test things or scrape information for you — and, more aggressively still, letting it drive your mouse and keyboard directly, operating the whole operating system. This course doesn't touch that layer.

- Search terms: `MCP server`, `browser automation agent`, `computer use agent`
- One-line prompt: "I already use an Agent desktop app for everyday work. Explain what MCP is, what extra things it lets my Agent do, and give me two examples a non-programmer would actually use."

**Direction three: take Agent Skill deeper.**

In Task 05 or Task 06 you only used a bare-bones summarize skill. There's no ceiling on this one: a Skill can package prompts, reference material, scripts, and tools, and several Skills can be chained together to do something big.

- Search terms: `Agent Skills`, `SKILL.md`, `awesome agent skills`
- One-line prompt: "I want to build my own Agent Skill for a kind of work I do over and over. Ask me a few questions first to pin down the boundary and the output standard for it, then write it for me."

And remember this one line: **basically anything a human can do, AI can do too, and it will probably do it better than a human most of the time.** You're only just getting started, but you've already pushed the door open.

---

## 11. Bringing Back Task 08's Mindset

The eight things above and those three directions are just a map of the tools. What actually determines your efficiency is the mindset from [Task 08](../08-plan-and-delegate/README.md): when context is going to get lost, solve it by writing a planning document; when you've got several things to do at once, first sort out which are exploratory and which are execute-and-review; do exploratory work in sequence and stop once an idea is about 70% baked; run execution work across several sessions at once, switching between them, playing the boss who checks on progress.

Tools will change, versions will get upgraded, interfaces will get redesigned. But this picture — the eight-thing foundation plus the mindset for directing the work — should still hold up on basically any new Agent App that comes along. That's the thing this course actually wants to leave you with.

---

## 12. From Task 02 to Here, the Full Picture of the Course

- [Task 02](../02-why-learn-this/README.md): why it's worth spending time up front learning to use an AI Agent, and this course's scope and boundaries.
- [Task 03](../03-model-chatbot-agent/README.md): the base model, chatbot, Agent framework, and where your money is actually going.
- [Task 04](../04-signup-and-pick-your-tool/README.md): picking one of the three tools based on your situation, and getting a free account set up.
- [Task 05](../05-claude-code/README.md): getting started with Claude Code Desktop, from picking a folder to using your first Agent Skill.
- [Task 06](../06-codex/README.md): getting started with Codex Desktop, from adding a project to using your first Agent Skill.
- [Task 07](../07-antigravity/README.md): the Antigravity piece isn't open yet, use the Codex piece as a reference for now.
- [Task 08](../08-plan-and-delegate/README.md): the mindset for planning, splitting up work, and running several sessions at once.
- Task 09 (this piece): pulling all of the above into one full picture, closing out the course.

---

## 13. Words from the Instructor

**Why this piece matters:**

Every earlier piece taught you one concrete thing — one tool, one feature, one piece of mindset. This one doesn't teach anything new; it teaches you how to look at everything you've learned as a whole. Looked at that way, you'll find you've learned more than you thought, and it's more broadly useful too.

**Key insight:**

- Specific tools will keep getting replaced one generation after another, but these eight things and the mindset from Task 08 are the foundation underneath all of them, and they won't go out of date easily.
- You don't need to master every direction for leveling up to consider yourself done. Knowing they exist, and knowing which level you're standing on right now, is already enough.
- If you want to go further, the cheapest path is reading the official docs rather than hunting for more second-hand tutorials. That used to be expensive. With an Agent reading alongside you, there's no longer a good reason not to.

**Closing note:**

That's it for this course. Where you go from here is up to you: keep going deeper with the tool you already have, go try the other one you haven't touched yet, or start exploring in a more professional direction. Whichever path you take, the picture you're carrying with you will still be useful.
