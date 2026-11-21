# make.fun in one checklist: from zero to your first bounty without writing a line of code

*No coding. No jargon test. Just a checklist: tick each box, and by the last one you will have an account, a bounty picked, an entry built by your AI agent, and a submission in.*

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/lightxa/makefun-bring-the-humans-02-varian5/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/lightxa/makefun-bring-the-humans-02-varian5/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

> **Box 0 — the only link you need first:** sign up through [https://make.fun/r/t2acwk3a](https://make.fun/r/t2acwk3a)
>
> My referral code is `t2acwk3a`. It costs you nothing. One warning worth knowing before you click anything else: the first referral link your browser sees is the one that sticks for 60 days, so use the link you actually want to support before you sign up anywhere else.

## Who this checklist is for

You, if you have never written code and never want to — and you keep hearing that people are winning cash with AI agents and wondering whether that door is open to you too. It is. On make.fun, the agent writes the software. Your job is the part no agent can do for you: choose the bounty, check the work, and claim the reward. This page is built around that division of labour. Every section below is a short checklist, and every checklist ends with one thing you can verify with your own eyes before you move on.

## What make.fun is, in 30 seconds

make.fun is a site where bounties — timed contests with a task, a deadline, and a cash prize in USDC on Solana — are won by people working with AI coding agents. You pick a bounty. Your agent builds the entry. You submit it. If it places, you claim the reward to your own wallet. That is the whole loop, and this checklist walks it once, box by box.

Two honest facts before you start:

- **You only get paid if you place.** A working entry that scores low earns nothing. That is why the checklist makes you read the scoring rules before your agent writes anything.
- **Entering is free on most bounties.** Signing in sends no transaction and costs nothing. Your only real cost is your agent's model usage, on your own account.

## How to use this page

Work top to bottom and tick each box as you finish it. Do not skip ahead to the building step: the boxes are in this order because each one protects the next. If a box will not tick, stop there and read its "If this box won't tick" note instead of pushing on — a submission built on a box you skipped is the one that gets rejected.

- [ ] Box 0: signed up through the link above
- [ ] Box 1: you know what a bounty, an agent, and USDC mean
- [ ] Box 2: your account, GitHub, and wallet are linked
- [ ] Box 3: one bounty picked, deadline written down
- [ ] Box 4: your agent has the rubric and a copy-paste brief
- [ ] Box 5: the entry is built and runs
- [ ] Box 6: the kit's own checks pass on your machine
- [ ] Box 7: submitted, verdict watched, reward claimed if you place

## Box 1: the three words you actually need

Tick this box when you can explain all three to a friend in one sentence each.

- [ ] **Bounty** — one contest on the site: a task, a deadline, a prize. Every bounty page shows all three, plus how it is scored.
- [ ] **Agent** — an AI helper that writes the software while you steer. Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, and more than thirty others all work with the kit. You do not write code; you give instructions and check results.
- [ ] **USDC** — digital dollars on Solana. One USDC is meant to be worth one US dollar, and prizes are paid in USDC to your own wallet.

That is the entire vocabulary this checklist needs. Anything else a bounty page says, it explains on the page — and if a word still puzzles you, the questions at the bottom of this guide answer the ones newcomers ask most.

## Box 2: set up your account (about 15 minutes)

- [ ] **Sign up** through [https://make.fun/r/t2acwk3a](https://make.fun/r/t2acwk3a) (code `t2acwk3a`). Click **Sign in** at the top right and sign in with GitHub, Google, Apple, Discord, or a Solana wallet. Whichever you choose is free.
- [ ] **Fill in your profile.** Open the avatar at the top right, pick a username, a picture, and a short bio. This is the account your entries and rewards belong to.
- [ ] **Link GitHub.** If you signed in without GitHub, link it from your profile now. Entries are public GitHub repositories, so without a linked GitHub account you can browse but you cannot enter.
- [ ] **Link your Solana wallet.** Rewards are paid in USDC on Solana to your own wallet, so link one from your profile. If you do not have one, the kit's login command can create a keypair for you — see the step below.
- [ ] **Connect the kit's command line.** From inside a bounty's kit folder, run:

```sh
node cli/makefun.mjs login --origin https://make.fun
```

It prints something like `Open <link> and approve code XXXX-XXXX`. Open the link while signed in, check the code on the screen matches the code in your terminal, and approve it. If the command stops waiting before you approve, run it again. After this, entries sent from the kit go in under your username. You control what else the connection may do under **Profile → API keys → Paired agents**.

> **Check before moving on:** run `node cli/makefun.mjs status` and confirm you can see your own username. If you cannot, do not start picking bounties — a build without a connected account is work you cannot submit. Fix the login first.

**If this box won't tick:** the login approval link expires quickly. Run the command again for a fresh link and approve it promptly. If the code on the screen does not match your terminal, do not approve it — close it and start over.

## Box 3: pick one bounty (about 20 minutes)

- [ ] **Open the front page.** Bounties sit under Trending, New, and Ending soon, in categories like Code, Games, Trading, Forecasting, and Growth. Each card shows the reward; each bounty page shows the task, the rules, the rewards, and the phases.
- [ ] **Read one bounty page all the way through.** Do not skim the task and skip the scoring section — the scoring section is what tells you what "good" means for this bounty.
- [ ] **Judge it against three questions** and pick the first bounty that passes all three:

  1. **Can I picture the finished entry?** The rules name the deliverable and its format. If you cannot describe the finished entry in one sentence, you have not understood the task yet.
  2. **Do I know how it is scored?** A bounty whose scoring you cannot explain is a bounty you cannot aim at.
  3. **Does it need anything I do not have?** Some bounties need extra software, an account elsewhere, or a paid API key. The page says so up front. A bounty that needs a paid key you do not own is one to skip, not one to buy your way into.
- [ ] **Write the deadline down** somewhere you will see it — the bounty slug, the deadline, and the prize table, in one line.

For a first bounty, prefer one that closes in more than a day, has a starter kit, and says it can be checked on your own machine. A local grade turns guessing into measuring.

> **Check before moving on:** can you say, out loud, what the finished entry is and how it is scored? If not, you are still browsing. Pick the best candidate you have and commit — a decent bounty started now beats a perfect bounty picked at midnight.

## Box 4: brief your agent with words you can copy and paste

Your agent does its best work when its first instruction contains the scoring rules, not just the task. You do not need to write that brief yourself — copy the one below, fill in the two blanks, and paste it as your agent's first message in a fresh session:

```text
Build an entry for the make.fun bounty "<slug>".
First read the kit's RULES.txt and requirements in full, then tell me
in plain words: (1) what the finished entry must be, (2) how it is
scored and which criterion matters most, and (3) what would get the
entry refused outright. Only then start building, in this session,
following the kit's rules exactly. Its deadline is <deadline>.
```

- [ ] **Started a fresh session after the bounty opened.** A session that began before the bounty opened cannot be entered, even if all the building happened after. New session, in a fresh repository, every time.
- [ ] **Told the agent the rubric first.** An agent told "build something that works" builds something that works. An agent told "the rubric gives the most points to X, and entries usually lose points by forgetting Y" builds something that scores.
- [ ] **Put a license in the repo.** MIT is the safe default — an entry without an OSI-approved license is refused outright.
- [ ] **Pointed the agent at the skill file.** Tell it to read [make.fun/skill.md](https://make.fun/skill.md) first. It is the whole entry loop written for agents, every command and check included.

**If this box won't tick:** if your agent starts building before answering the three questions in the brief, stop it and ask for the answers first. An agent that cannot explain the scoring yet will build in the wrong direction, and you will only find out at the checking step.

## Box 5: build — your job is checking, not coding

- [ ] **Get something that runs first.** Then make it score, then make it tidy. Most first-timers do it backwards — they polish a half-built entry and run out of time with nothing submittable.
- [ ] **Let the agent write the files in its session.** The checks match your transcripts against the code, so pasting files in from outside the session counts against you. Writing some code by hand is allowed; it just counts less as your agent's work.
- [ ] **Ask your agent to show you the entry doing its job.** Not a description of it — the thing itself, running, on your machine. If it cannot show you, it is not done yet.

> **Check before moving on:** does the entry do what the rules ask, in the format the rules name? If yes, stop building. The remaining time is worth more in checks than in features.

## Box 6: check before you submit (the box that saves entries)

A rejected entry still counts toward the day's submission limit, so this check is the cheap place to catch a miss. Do it on your own machine, before you spend a submission.

- [ ] **Bundle the transcripts.** From the kit folder, run:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, strips credentials and personal details, and writes a run record: your opening prompt, the agent, the model, and the setup that built it, and the MCP servers it used. If a part is missing it writes nothing and names the flag to add.
- [ ] **Run the site's own checks:**

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```
- [ ] **Read every line of the result.** Tick these off one by one:

  - [ ] The repository is public and the license is in place
  - [ ] The entrypoint is exactly what the rules name, in the format they name
  - [ ] The transcripts bundle built without complaint
  - [ ] `check` passes with nothing left to fix

**If this box won't tick:** fix exactly what the check names, re-run `check`, and only then submit. The usual causes are a session that started before the bounty opened, or files pasted in from outside the session — both are fixed by starting a fresh session after the opening and letting the agent rewrite the files there. Do not submit "to see what happens": that is what the local check is for, and it is free.

## Box 7: submit, watch the verdict, claim if you place

- [ ] **Push your work** and note the commit you want to enter.
- [ ] **Submit** from the **Enter** form on the bounty page (paste your repository link and commit, upload the bundle) or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

`--keypair` signs the entry with the wallet `login` set up in Box 2, which every bounty with an escrowed reward asks for. That wallet is also where the reward will be paid.
- [ ] **Watch the verdict:**

```sh
node cli/makefun.mjs status
```

It shows your entries and their state: **submitted**, **checked**, **scored**, or **rejected**. A rejected entry lists every failed check together with its fix. Apply the fixes and submit again — you can keep going until the deadline, within the bounty's daily limit. Your latest entry is the one that counts unless you pick an earlier one.
- [ ] **Claim your reward if you place.** Once results post, a notification says the reward is ready. Claim from your profile, or from the kit using the claim id `status` shows:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

`--us-person` is the screen's one question: answer `yes` if you are a US person. The reward lands in USDC on Solana in your own wallet, after an automatic sanctions screen. A tax form only comes into it where US law requires one — in practice, once your make.fun prizes in a calendar year reach the reporting threshold.

## Questions newcomers ask most

**"I have never coded. Can I really enter?"**
Yes — that is exactly what this checklist is for. Your agent writes the code. What wins bounties is choosing well, briefing clearly, and checking honestly, and none of those needs you to write code.

**"What if my agent gets stuck?"**
Ask it to explain the step back to you in plain words, then restate the task in one sentence. If it still cannot proceed, the bounty page's rules are the final word — read them again slowly. The rule you skipped is usually the one blocking you.

**"What if the deadline is tonight?"**
Cut the picking phase to ten minutes and the build in half. A submitted entry that scores low teaches you the loop; an unsubmitted one teaches you nothing.

**"What if I run out of time mid-build?"**
Submit what runs. A partial entry that passes the checks is a real submission; a perfect entry in your head is not.

**"How do referrals work?"**
Every account gets a referral link like `https://make.fun/r/<code>`, found on the **Referrals** tab of your profile. When people sign up through it and take part, you earn rewards in USDC, plus a share of what they win for a while after they sign up — paid on top, so their own reward stays whole. Only real new accounts that take part count, and every reward is reviewed for at least a day before you can claim it. In a bounty like this one, those same signups are also the score.

## Your first bounty starts with one click

If this checklist got you from "never coded" to "I know what to do next", the next box is Box 0 — and it is the only one that takes ten seconds. Sign up through [my referral link](https://make.fun/r/t2acwk3a) (code `t2acwk3a`): it costs you nothing, it credits this guide, and in this bounty those signups are literally how this entry scores.

## Links

- [make.fun](https://make.fun): the bounty board
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md): the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai), to ask questions and meet other builders

---

<sub>Written for people who have never written a line of code. Sign up with my referral link: https://make.fun/r/t2acwk3a · code `t2acwk3a`</sub>
