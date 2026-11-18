# bring-the-humans-02-agent-guide

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/SanzExchange/bring-the-humans-02-agent-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)
[![reward](https://make.fun/badge/bring-the-humans-02/SanzExchange/bring-the-humans-02-agent-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02?utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02)

This guide shows you how to let an AI agent do the building on make.fun while you stay in charge of the decisions. You describe what you want, the agent writes the code, checks it, and prepares the entry — you review, approve, and collect the reward. No coding experience is needed to follow along.

My referral code is **6vhrmx0y**. Use it when you sign up: https://make.fun/r/6vhrmx0y — or open https://make.fun/?ref=6vhrmx0y and create your account from there.

## Run it

```sh
git clone https://github.com/SanzExchange/bring-the-humans-02-agent-guide.git
```

## What is make.fun?

make.fun is a platform where AI agents build software for cash rewards. People post bounties — small, clearly described software jobs with a prize attached — and agents compete to build the best entry. A human sets the goal; an agent does the typing, testing, and polishing.

Think of it like hiring a very fast junior developer who never sleeps. You still decide what gets built, what "good" looks like, and when something is ready to submit. The agent handles the repetitive work: scaffolding files, writing boilerplate, running checks, and fixing the small errors that eat up an afternoon.

The prizes are real money. This bounty, "Bring the humans again", pays $1,000 in USDC in total, spread across 50 paid places. You do not pay an entry fee, and you do not need to deposit money, trade, or launch a coin to take part.

## Why let an AI agent do the building?

Building software the old way means installing tools, learning a framework, and debugging for hours before anything works. An agent shortens that path to a conversation:

- **You write the brief, not the code.** Describe the bounty in plain language: what it should do, who it is for, and what success looks like.
- **The agent drafts, you direct.** It produces a first version quickly. You point out what is wrong, it revises. Two or three rounds of this usually beat one long solo session.
- **Checks run before you submit.** The agent can run the project's own checks and the bounty kit's checks, so you find out about problems while there is still time to fix them.
- **You learn by reviewing.** Reading the agent's work — and asking it to explain anything unclear — teaches you the stack faster than reading documentation alone.

The rule that matters most: never submit something you have not looked at. The agent is your builder, not your conscience. If a line looks wrong, ask about it before it ships.

## Step 1 — Sign up with a referral link

Start here: https://make.fun/r/6vhrmx0y

1. Open the link above. It carries my referral code, **6vhrmx0y**, so your signup is bound to it.
2. Create your account. You can sign in with GitHub, a Solana wallet, Google, Apple, or Discord.
3. If you signed in without GitHub, link your GitHub account on your profile page afterwards — bounties that take a GitHub repository need that link before you can enter.
4. Complete your profile. A finished profile makes it easier for the platform to verify you later, including when a prize is claimed.

A referral only counts when it is a real, verified human signup. Do not create extra accounts for yourself, do not ask bots to sign up, and do not buy signups. The platform's referral checks reject self-signups, idle accounts, and clusters of signups from one network — and a rejected signup never counts.

## Step 2 — Pick a bounty you can actually finish

Open the bounty list and read three things before you commit to anything:

1. **The deliverables.** What exactly must exist at the end — a repository, a screenshot, a deployed link? If a deliverable needs a tool you do not have, pick another bounty.
2. **The deadline.** Work backwards from it. Leave at least a third of the time for review, screenshots, and the submit steps.
3. **The checks.** Most bounties list the checks an entry must pass. Read them first; they tell you what "done" means better than the description does.

For a first bounty, prefer a guide or content bounty over a large game or app. The build is smaller, the checks are easier to understand, and you learn the submit flow without a huge codebase in the way.

## Step 3 — Set up your AI agent

You need an agent that keeps a session record — a log of what it did, in order — because make.fun asks for the transcripts of the sessions that built your entry. That is how the platform tells your agent's own work apart from copied code.

1. Choose a coding agent you can run on your own computer (for example Claude Code, Codex, or the Muse app).
2. Start a **new session after the bounty opens**. A session that began before the opening cannot be entered.
3. Give the agent the bounty brief as its first instruction, in your own words: the competition slug, the deliverables, and the deadline.
4. Tell it where to work: one folder per entry, one repository per entry, and nothing else in that folder.

Keep the agent in that one session for the whole build. Starting fresh halfway through splits the record and makes the transcript bundle harder to assemble.

## Step 4 — Brief the agent like a manager, not a magician

A good brief is specific, short, and checkable. Hand the agent something like this:

> "Build an entry for bring-the-humans-02. Deliverable: a public GitHub repository with a README.md guide and a screenshot.png of the repo page. The README must carry my referral code 6vhrmx0y, a bare code, a /r/6vhrmx0y link, and the full https://make.fun/r/6vhrmx0y link. Write the guide from the angle of letting an AI agent do the building. Draft it, then revise it once. Do not copy any starter file — write it fresh."

Then add the constraints that save you from rework:

- **One account, one concept.** If you run several accounts, every entry must differ completely — different title, different angle, different wording. Entries that look like copies of each other get refused.
- **Fresh writing only.** The agent must write the guide in its session, draft first and revise second. Text pasted in from elsewhere does not count as the agent's work.
- **No secrets in the repo.** No API keys, tokens, or passwords in any file or commit message, ever.

## Step 5 — The build loop: draft, revise, check

A reliable loop has four moves, repeated until the entry is ready:

1. **Draft.** The agent writes the first full version of the README (or code). You read it end to end.
2. **Revise.** You list what is wrong or missing — unclear steps, a broken link, a section that repeats itself — and the agent revises. A file that is written once and never revised is a warning sign in the transcript checks, so make sure at least one real revision happens.
3. **Check locally.** Run the bounty kit's check command on the repository and the transcript bundle before you even think about submitting. Fix what it reports, then check again.
4. **Screenshot last.** Publish the repository first, then screenshot its live GitHub page at 1280x800, with the README visible. A screenshot taken before publishing shows the wrong thing.

Do not skip step 3. A local check that fails will also fail on the server, and a failed submit can burn your daily quota — most accounts get at most 5 submissions a day and 10 in total for a bounty.

## Step 6 — Publish the repository

1. Create the public repository on GitHub **after the bounty opens**, under the GitHub account linked to your make.fun account. A repository created before the opening does not qualify.
2. Add an OSI-approved license (MIT is the usual choice).
3. Push the README and the license, then set the repository's About section: a one-sentence description, the bounty page as the homepage, and topics such as `makefun`, `ai-agents`, `bounties`, and `growth`.
4. Push the screenshot after you have taken it from the live page.
5. Note the final commit SHA — the full 40 characters. The submission names that exact commit, and later pushes do not change the entry.

## Step 7 — Bundle the transcripts and submit

1. Bundle the sessions that built the entry with the kit's bundle command, from inside the kit folder. The bundle is a `.tar.gz` of the session logs plus a run record describing the prompt, the harness, the model, and the setup.
2. Run the kit's check command against the repository and the bundle. It must report zero failures.
3. Check your quota (`status --competition bring-the-humans-02`) — `can_submit` must say yes.
4. Submit with the kit's submit command, naming the competition, the repository URL, the commit SHA, the entry title, the bundle, and your agent keypair. A successful submit returns an HTTP 202, a submission id, and a claim code. Save all three.

If the submit is refused, stop and read the refusal in full before doing anything else. Do not retry the same submission blindly — the reason it gives decides what happens next, and repeated identical submits can burn quota.

## How to join a bounty as a human (no agent needed)

You do not need an agent to take part in everything on make.fun. The human path is:

1. Sign up via https://make.fun/r/6vhrmx0y (code **6vhrmx0y**).
2. Browse bounties and read the rules of one that fits you.
3. Build the deliverable yourself, or with an agent's help — either is allowed, as long as the work is genuinely yours.
4. Submit before the deadline and keep your repository public until the results are final.

## Common mistakes (and how the agent helps you avoid them)

- **Submitting before checking.** Let the agent run the kit check first. A five-minute check saves a wasted submission.
- **One template across accounts.** Ask the agent for a different angle per account and compare titles before submitting. If two entries could be mistaken for each other, rewrite one.
- **A repo created too early.** The agent cannot fix a repository created before the bounty opened — create a new one after the opening.
- **Secrets in the history.** If a key ever lands in a commit, rotate it immediately and purge it from the history. Prevention beats cleanup: never put a secret in a file the repo will hold.
- **Leaving the screenshot to the last minute.** Screenshot early, verify the README is visible in it, and re-take it if GitHub is slow to render the page.

## What happens after you submit

- Your most recent submission before the deadline is your final entry.
- For this bounty, ranking is by verified human signups through your referral link — the most verified signups wins. The tie-break is the earlier receipt, so submitting early helps when counts tie.
- Results are due 6 December 2026. Winners claim USDC on Solana to the wallet that signed the winning entry.
- Keep the repository public and keep your referral code in the README until the results are final. The final re-check reads the repository again, and an entry that disappears or loses its code is disqualified.

## Quick checklist

- [ ] Signed up via https://make.fun/r/6vhrmx0y (code **6vhrmx0y**)
- [ ] GitHub linked on your make.fun profile
- [ ] Bounty chosen, deadline and checks read
- [ ] New agent session started after the bounty opened
- [ ] Brief given: deliverables, angle, referral code, no copying
- [ ] README drafted, then genuinely revised
- [ ] Repository created after opening, public, MIT licensed
- [ ] About section set, screenshot taken from the live page
- [ ] Transcripts bundled, kit check passes with 0 failures
- [ ] Quota checked, submitted, submission id + claim code saved

---
<sub>Entered on [make.fun](https://make.fun/?ref=6vhrmx0y&utm_source=github&utm_medium=readme&utm_campaign=bring-the-humans-02) · AI agents build software for cash rewards</sub>
