---
description: "By the end you can clearly explain what a foundation model, a ChatBot, and an Agent each are, why Agent equals foundation model plus Harness, why these Agents all got their start writing code, the difference between CLI and Desktop, what you are actually paying for, and where something like OpenClaw fits in the picture."
---

# Foundation Models, ChatBots, and Agents: the Skeleton Behind All of This

> Nail these few terms once, and every article after this one will make a lot more sense.

## 1. Overview

The last article covered "why learn this." This one covers "what exactly are you using."

Whether you end up installing Claude Code, Codex, or Antigravity, the same skeleton holds all of them up underneath. Rather than re-explaining it in every article, let's get it straight once, right here. Foundation model, ChatBot, Agent, Harness, CLI, Desktop — understand these terms once and you'll never get confused by them again.

This one doesn't require you to do anything hands-on either. Just spend twenty minutes and get the concepts straight in your head.

---

## 2. Learning Goals

What does it cost you if you never get this skeleton straight? You'll never be sure what you're actually paying for. You'll assume switching software means switching to a different AI. You'll get yanked around by every new buzzword, and panic a little every time a new product ships, wondering if you've fallen behind again.

Once the skeleton is in place, all that noise goes quiet. You'll notice that most of what looks like a brand-new thing is really the same handful of building blocks, rearranged. That's where judgment comes from.

By the end of this task, you'll be able to:

1. Explain the relationship between foundation model, ChatBot, and Agent, and why Agent equals foundation model plus Harness.
2. Explain why these Agents all got their start writing code, and the difference between the CLI and Desktop forms.
3. Explain exactly what you're paying for, and where something like OpenClaw fits in this picture.

---

## 3. Prerequisites

- You've read Task 02 and know what this course covers and where its boundaries are.
- No programming or tech industry background required.

---

## 4. What You'll Learn

A skeleton diagram, a timeline, and a piece of judgment. After reading this, you'll be able to place any newly hyped AI product in just a few sentences.

---

## 5. Foundation Model: the Brain Behind the Whole Thing

At the core of everything is the **foundation model** (also often called a "large model" or "base model").

Think of it as the brain of the entire AI stack. When you ask it a question, it thinks, it answers, it writes things, it does work for you — all of that runs on this brain. As the last article mentioned, only three companies in the world have made it into the first tier of foundation models: OpenAI (its models are the GPT series), Anthropic (its model is called Claude), and Google (its model is called Gemini).

Remember this one fact, and a lot of later confusion resolves itself: **the thing that's genuinely valuable, the thing that actually costs money, is the brain.** All the different software, interfaces, and flashy products you'll run into later are just different ways of using and wrapping that same brain. There are only a handful of brains. There can be endless layers of shells around them.

---

## 6. ChatBot: the First Shell You Ever Touch

Most people's first contact with AI is through chatting: you open a webpage, type into a box, and it types something back. That thing is called a **ChatBot**.

A ChatBot is the first, simplest shell wrapped around the brain. Whether you're chatting on claude.ai, chatgpt.com, or gemini.google.com, it's fundamentally the same thing happening: you type, your words get sent into that brain, the brain figures out an answer, and it gets displayed back to you.

It's easy to pick up, has a low barrier to entry, and works fine for casual questions or quick lookups. But it has a ceiling: it's basically "you ask one thing, it answers one thing." If you want it to actually carry out a complex task from start to finish on its own, chatting alone won't cut it. That brings us to the next, more important layer.

---

## 7. Agent: the Shell That Actually Gets Work Done

An **Agent** is an even more capable shell wrapped around the brain.

Here's the difference: with a ChatBot, you ask and it answers. With an Agent, you hand it a goal, and it breaks the goal into steps on its own, takes action on its own, and works through the task step by step until it's done. It can read files, edit files, run programs, check whether its own results are correct, and if it finds a mistake, back up and try again. This is the thing people mean when they say it can "get work done and solve problems better than most white-collar workers." And it can be customized — you can teach it how you want work done (remember Agent Skills from Task 02? That's exactly how you customize it).

So how does an Agent become this capable? At its core, it's a foundation model wrapped in a carefully engineered framework — one that lets the brain call tools, read and write files, hold onto context, and loop through self-correction. This framework has a specific name in the industry: **Harness**.

So remember this formula:

**Agent = foundation model + Harness**

Take the same brain, wrap it in a good Harness, and it goes from something that just chats to something that actually gets work done. That capable, work-doing Agent is exactly what this course is ultimately trying to get you using.

This formula also answers a question left open in the last article: why products like Cursor have a thin moat. It's because they're only building the Harness half — the brain half is rented. And between those two halves, the hard part, the expensive part, the part nobody can quickly copy, is precisely the brain half.

---

## 8. Why These Agents All Made Their Name Writing Code

You may have noticed something: the most famous Agents today all seem to talk about writing code, in their names and in their marketing. A lot of people conclude from this that these tools are for programmers, and have nothing to do with them.

That's a misunderstanding. **An Agent can fundamentally do almost anything** — writing code was just the first arena where it proved itself. Why coding specifically? Because **programming is the domain where right and wrong are easiest to verify.**

Think about it: if you had AI try to cure a disease, or run your company well, how would you even know, in the moment, whether it did a good job? There's no instantly checkable standard, and results take a long time to show up. Writing code is different: whether the code runs, whether the tests pass, whether the feature works — you know immediately. Right is right, wrong is wrong.

For a company trying to get its Agent to mature quickly, the choice is obvious: dive into an arena where you can verify results fast and objectively, use that to sharpen the Agent's real capability, and build your reputation along the way. That's why all these Agents started out with code.

But don't let that origin story mislead you: underneath, it's a general-purpose tool for getting things done, not a toy that only writes code. Use it to organize research notes, write documents, or do research, and it works just as well.

---

## 9. A Timeline: From Large Model to Super App

Put all of this on a timeline and the last few years turn out to have a pretty clear arc.

**Phase one: only the brain.** ChatGPT exploded onto the scene in late 2022, and for the first time the general public got their hands on a large model directly. For a year or two after that, the competition was purely about how smart the model itself was, and about all you could really do was chat.

**Phase two: crude Agents.** Around 2023, people started experimenting with letting models call tools on their own and loop through work on their own. The most famous attempt of that era was called AutoGPT. The idea was right, but the execution was rough: it would frequently go off the rails and unravel mid-task. It was more of a jaw-dropping demo than something you could actually rely on for real work.

**Phase three: the breakthrough.** By 2025, two things matured at the same time: the models themselves got strong enough to reliably handle multi-step reasoning and tool calling, and the Harness layer around them got polished enough to hold up. Agents became genuinely useful for the first time, and the breakthrough came exactly where the last section said it would: writing code.

**Phase four: everyone catches up.** Once one company cracked it, the other two followed fast. By late 2025, all three had shipped their own desktop Agent: Claude Code, Codex, and Antigravity. The landscape was set.

**Phase five: growing into a super app.** As of today, mid-2026, these tools have long since outgrown "just for writing code." They can read your files, browse the web for you, operate your computer, plug into your messaging apps, and work the way you've taught them to. They're turning into an entry point — the first place you go for anything.

Once you see this arc clearly, you'll notice every advance happened on one of the two halves of the same formula. Either the brain got stronger, or the Harness got better. It never stepped outside that frame.

---

## 10. CLI and Desktop: Two Faces of the Same Agent

The same Agent usually comes in two forms — two different ways of interacting with it.

One is called **CLI** (Command Line Interface). It looks like a plain black window full of text: you type a command, it types back. It looks this way because Agents were originally built for professional developers, who already live in windows like this all day. CLI is powerful and flexible, but for most people the learning curve is steep, and it's easy to be scared off at first glance.

The other is called **Desktop**. It's just ordinary software installed on your computer, with windows, buttons, and a chat box — not much different from any other app you already use. Point, click, and you're off.

Neither form replaces the other; each has its own strengths. CLI is more powerful and flexible for certain kinds of work, while Desktop is more intuitive and convenient for others. Worth noting: using Desktop is not "beginner mode." Plenty of professional developers spend a good chunk of their time working in Desktop too. It's a legitimate primary tool in its own right.

This course focuses on the **Desktop version**, the friendliest option for newcomers.

---

## 11. What You're Paying For Is Compute, Not Software

With all of the above in place, one thing that confuses a lot of people can now be explained in a single sentence: **what you're paying for is the compute behind that brain, not the software wrapped around it.**

Think about it: Agent software like Claude Code, Codex, and Antigravity is installed on your own computer and runs on your own computer. Running it burns your own hardware, not a cent of some company's data center — which is exactly why the software itself is usually free to download and free to install.

The brain is different. It's far too large to fit on your computer, so it has to live in OpenAI's, Anthropic's, or Google's data centers. Every time you make it think, every time you make it do work, real electricity gets burned and extremely expensive hardware gets tied up on their end. That's a real, hard cost. So it's always been the brain — its compute — that gets billed.

This also explains something else: why several upcoming articles spend real time on how to pick a subscription plan. You're not choosing a software edition. You're choosing how much compute you get to use.

---

## 12. One Step Further: Personal AI Operating Systems Like OpenClaw

Let's close with something you've probably already seen floating around Chinese-language corners of the internet: **"the crawfish."**

Its official name is **OpenClaw**, created by Peter Steinberger, open source, and installed on your own machine. It's been renamed a few times: it started out as Clawdbot, then was briefly called Moltbot after being asked to change its name because it sounded too close to "Claude," and finally settled on OpenClaw at the end of January 2026. So you'll see different names for it depending on when an article was written — they're all the same thing.

How is it different from a tool like Claude Code? Claude Code is something you open when you want to use it. OpenClaw, by contrast, is an always-on Gateway that plugs into a whole pile of your messaging channels — WhatsApp, Telegram, WeChat, Feishu, and more — so wherever you happen to send it a message, it goes and does the work on your machine. That makes it feel more like an operating system than an app. There's a Chinese counterpart in the same category too: NetEase Youdao's LobsterAI.

There's another notable name in this same category: **Hermes Agent**, from Nous Research. It takes a different approach: instead of stacking up more channels, it stacks up self-improvement — every time it finishes a task, it distills a new Skill from the experience, so it does better next time.

How should you place things like this? Now that you have the skeleton, it takes one sentence: they're essentially **customized, more elaborate versions of Claude Code / Codex / Antigravity**. Underneath, it's the exact same formula — foundation model plus Harness — just with the Harness layer built out much bigger, more like a platform. This course won't go into them in depth.

So should you actually chase after them? Here's a rule of thumb. If you're an employee at a company, Claude Code, Codex, and Antigravity already cover 99% of your work, and you don't need to worry about anything else. If you're a founder, these AI-operating-system tools might get you an extra 5% to 10% that those three tools can't reach on their own. But the flip side holds too: even for a founder, getting genuinely good at those three tools alone covers more than 90% of what you'll ever need.

So the takeaway is simple: get the foundation solid first. Once the foundation is solid, everything you add on top comes fast.

---

## 13. Exercises

### Exercise 1: Explain the Skeleton in Plain Language

**Goal:** Test whether you actually understood this, or just read it.

**How:**

1. Find someone who knows nothing about any of this — a family member, a friend, anyone — or just talk it out loud to a voice recording.
2. In under three minutes, explain four things: what the brain is, what a ChatBot is, why an Agent beats a ChatBot, and where your money actually goes.
3. You're not allowed to use words like "Harness" or "foundation model." Plain language and analogies only.

**What you'll notice:**

Wherever you get stuck is exactly where you didn't really understand it. Go back and re-read that section.

> **Key insight:** Being able to explain it in plain language is what it means to understand it. Being able to repeat the jargon just means you've seen it before.

### Exercise 2: Place a Few Products on the Map

**Goal:** Put the skeleton to work as a measuring stick.

**How:**

1. List four or five AI products you've heard of — say, the claude.ai web app, Claude Code, Cursor, OpenClaw, and anything new you've stumbled across recently.
2. For each one, answer three questions: Is it a ChatBot or an Agent? Whose brain is it running on — its own, or rented? Is it CLI or Desktop?
3. If you can't answer, check the product's website — it usually only takes a few minutes to find out.

**What you'll notice:**

Most products can be cleanly placed using these three questions. The ones you can't place are usually just buried under thick marketing language, not doing anything technically new.

> **Key insight:** Once you have the skeleton, you don't need to chase the news anymore. Any new product that shows up, measure it against this yardstick, and three sentences will tell you what it actually is.

---

## 14. Recap: What We Learned

- The foundation model is the brain. Only three companies in the world are in the first tier: OpenAI, Anthropic, and Google. The brain is what's valuable.
- ChatBot is the simplest shell: you ask, it answers.
- Agent is the shell that gets work done. The formula is foundation model plus Harness. It breaks work into steps, takes action, and corrects itself on its own.
- These Agents all got their start writing code purely because programming is the easiest domain to verify right and wrong in on the spot — that doesn't mean it's all they can do.
- The timeline: only the brain, crude Agents, the breakthrough, everyone catches up, growing into a super app. Every step happened on one of the two halves of the formula.
- The same Agent comes in CLI and Desktop forms, each suited to different situations; this course teaches Desktop.
- What you pay for is the brain's compute; the software itself is usually free.
- Personal AI operating systems like OpenClaw and Hermes Agent are, at their core, more elaborate customized versions of the same Agent formula. Get genuinely good at the three mainstream tools first, and that covers more than 90% of what you'll need.

---

## 15. A Note from Your Mentor

**Why this article matters:**

You finish this piece with nothing new in your hands: no files, no output, just one more picture in your head. But it's the highest-value twenty minutes in the whole course.

Because the most exhausting thing about the AI field isn't that it's hard to learn — it's the constant low-grade anxiety of being bombarded with new buzzwords every day: another new thing just shipped, am I falling behind again? The skeleton is the cure for that. Once you have it, new products stop looking like a wall of unfamiliar names and start looking like a few familiar building blocks, rearranged.

**Key insights:**

- Shells come and go in waves; there are only ever a handful of brains. When you're deciding whether a product deserves your time, check first whether it has its own brain.
- Every so-called major breakthrough, once you take it apart, turns out to be one half of this formula getting stronger. Once you know that, marketing language has a much harder time fooling you.

**What's next:**

Now that you have the skeleton, it's time to pick a side. Task 04 will help you lock in which of Claude Code, Codex, or Antigravity to learn, based on where you live and what your career goals are. Once you've picked, you only need to read the track that applies to you — feel free to skip the rest.
