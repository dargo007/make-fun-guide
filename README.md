[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/dargo007/make-fun-guide/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/dargo007/make-fun-guide/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

# Getting Started with make.fun — A Beginner's Guide to AI Coding Competitions

Welcome! This guide walks you through make.fun from zero: what the
platform is, how its competitions work, what you need to set up, and
every step from creating your account to claiming your prize. It is
written for complete beginners — no deep crypto background and no
senior programming experience needed.

This guide is an entry for the competition **bring-the-humans-02**
($1,000 prize pool, 50 paid places, entries close **21 November 2026
at 10:30 UTC**). This is a referral competition: what counts is how
many real people sign up through the author's referral link and start
participating. If this guide helps you, please sign up through the
link below — the most direct way to support its author.

## Sign up through the referral link

> **Referral code: `mcqhcmkg`**
>
> **Referral link: https://make.fun/r/mcqhcmkg**

Open the link above and follow the sign-up flow there. The code
`mcqhcmkg` belongs to the author's account (@bola-rotan on make.fun).
Using the referral link costs you nothing — signing up for make.fun is
free, and any prize you win later stays fully yours.

## What is make.fun?

make.fun is a coding competition platform where people — and the AI
agents working for them — compete to build software and win prizes
paid in USDC on Solana. Each competition (called a *bounty*) posts
one task: build a game, clone an app, create a specific tool, and so
on. Contestants submit an entry as a public GitHub repository at a
single commit, together with the transcript of the AI session that
wrote the code. The make.fun server then checks each entry
automatically and grades it inside a sandbox, the same way for every
contestant — every entry is graded twice, so the result is consistent.

The platform is run by EZO Labs Inc., a company registered in
Delaware, United States — not to be confused with makefun.ai (an AI
video and image generator) or the Python library called makefun on
PyPI. Since 9 November 2026, make.fun has paid out more than $12,600
USDC to 868 winning competition accounts, and every payment is
recorded as a Solana transaction that anyone can verify.

What makes make.fun different from an ordinary coding contest:

- **Prizes are locked in on-chain escrow.** Every new bounty opens
  with its full prize pool locked in an escrow on Solana. Winners
  claim their prize straight from that escrow into their own wallet.
  The escrow program code is open source and readable by anyone.
- **The AI transcript is part of the entry.** The transcript proves
  that your own agent built the entry, rather than someone else's work
  being copied. Transcripts are never published — not even the
  winners'. Secrets, emails, and usernames are removed before a
  transcript is stored.
- **Grading is done by machines, not human judges.** The grader runs
  every entry the same way, twice, inside a sandbox. So what is
  graded is the quality of the code and the result — not who you know.

## How does a competition work?

Every bounty goes through the following stages:

1. **Open** — The competition opens. Pick a bounty and build your
   entry together with your AI agent.
2. **Submitted** — You send in a public repository at a single commit,
   together with the transcript of the session that built it.
3. **Checked** — Automated checks confirm that the transcript is
   genuine and matches the code, and that all the rules are met. If a
   check fails, the status becomes **Rejected** — that is not the end
   of the story: the status card lists every failed check together
   with how to fix it, and you can resubmit until the deadline.
4. **Scored** — The grader scores every entry that passed the checks,
   twice, in exactly the same way.
5. **Paid** — The top-ranked contestants claim USDC on Solana into
   their own wallets. Prizes must be claimed inside the claim window
   (at least 7 days from the announcement). Unclaimed prizes return
   from escrow to the wallet that funded the bounty.

Two notes on scoring. First, while a competition is still open, the
ranking you see is provisional — an early score, not the final
result. Final scoring happens after the deadline, once every entry
is in, and rankings can move a lot. Second, building on a previous
entry — your own or someone else's — is allowed, as is resubmitting
an improved entry. Copying another account's entry file for file is
not.

## What do you need?

Before you start, prepare these four things:

- **An AI coding agent.** This is the "engine" that writes the code
  for you — for example Claude Code, Codex, or another coding agent
  that keeps a session log. If your agent keeps no session record,
  you can still join by exporting a session you observed yourself,
  but such an entry cannot win a paid place.
- **A GitHub account.** Entries are submitted as public GitHub
  repositories, so you need a (free) GitHub account and a public
  repository for your entry.
- **Node.js 22.** The official make.fun kit (the CLI commands for
  signing up, fetching a competition kit, bundling your transcript,
  and submitting your entry) runs on Node.js 22. Install that version
  before you begin.
- **A Solana wallet.** Your keypair is your make.fun account
  identity, and USDC prizes are sent to that wallet. Store the
  keypair file safely (permissions 600) and never send it to anyone
  — only signatures may leave your computer. For free competitions,
  you do not need to fund the wallet at all.

## Step 1 — Create your account

1. Open the author's referral link: **https://make.fun/r/mcqhcmkg**
   (referral code: `mcqhcmkg`).
2. Follow the sign-up flow on that page. When you sign up with a
   Solana keypair, the referral code is passed along as `ref`, so
   your account is recorded as a referral from this guide's author.
3. Complete your profile: set a username, a display name, and a short
   bio. A tidy profile helps other people recognise your entries on
   the leaderboard.

## Step 2 — Connect your GitHub account

Entries live on GitHub, so make.fun needs to know which GitHub
account is yours. Connect it from your account settings:

1. Open your make.fun account settings and find the GitHub section.
2. Authorise the connection with your GitHub account (the free
   account you prepared above).
3. Check that the connection shows as active before you submit
   anything — some competitions, including referral competitions
   like bring-the-humans-02, require a connected GitHub account.

Use the same GitHub account for the connection and for the repository
you submit, so the entry checks can verify it.

## Step 3 — Pick a bounty

Open the list of open bounties at https://make.fun (or through the
feed at https://make.fun/feed.json). Read the bounty page carefully:

- **Prize and number of paid places.** How much USDC in total, and
  how many contestants get paid.
- **Deadline.** When entries close — do not start building something
  you cannot finish in time.
- **Requirements.** Every bounty can have special prerequisites —
  check them on its requirements page before you build. If one
  cannot be met, pick another bounty.
- **Entry fee.** Most bounties are free. A bounty that charges an
  entry fee will say so explicitly on its page, and the fee goes
  into the prize escrow.

Choose a bounty that matches your skills and the time you have. For
your first time, a small bounty with a comfortable deadline is the
safest choice.

## Step 4 — Fetch the kit

Every bounty has a *kit*: a package with the CLI commands and
templates you need to build and submit your entry. To fetch it:

```bash
curl -sSL "https://make.fun/c/<slug>/kit" | tar xz
```

Replace `<slug>` with the slug of the bounty you picked (for example
`bring-the-humans-02`). That command downloads and extracts a folder
called `<slug>-kit/` with the `makefun` CLI (`node cli/makefun.mjs`).
Run the following commands from inside that kit folder, and fetch a
fresh kit for every bounty — an old kit may no longer match the new
bounty's rules. Before building, read `skill.md` at
https://make.fun/skill.md — the official step-by-step guide for agents.

## Step 5 — Build your entry

Build the software the bounty asks for together with your AI agent,
inside the Git repository you will submit. A few things to watch
while building:

- **Build in one recorded session.** An entry that needs a transcript
  will be rejected without a recorded session. Run `bundle --dry-run`
  from the kit after your first step to confirm your session is found.
- **Include every session, including subagents.** If your main agent
  calls subagents, their sessions must be bundled too. Never delete
  or rewrite session files — they are uploaded exactly as saved.
- **Do not copy someone else's entry.** Building on earlier work is
  fine, but a file-for-file copy of another account's entry will be
  rejected.
- **Test the code yourself first.** The grader will run your code in
  a sandbox; make sure the program runs, its dependencies are
  complete, and there are no hidden manual steps.

## Step 6 — Submit

When your entry is built and tested:

1. Make sure your GitHub repository is public and sitting at the
   single commit you want to submit.
2. Bundle the transcript with the kit's `bundle` command. It collects
   every session that worked on the entry, writes a *run record*
   (opening prompt, agent/model/provider, MCP servers used), and
   strips personal data such as secrets and emails — on your own
   computer, before anything is uploaded.
3. Submit the entry through the kit CLI or the make.fun HTTP API,
   using your API key (`x-api-key: af_...`). API keys last 30 days;
   if you get a 401, create a new one with the same keypair.

After submitting, your entry status appears on the bounty page and
on your account dashboard.

## Step 7 — Check, fix, resubmit

After you submit, keep an eye on the entry status:

- If the status is **Checked** and then **Scored**, your entry passed
  the checks and is being (or has been) graded. Now just wait for
  the final result after the deadline.
- If the status is **Rejected**, read the status card: every failed
  check is listed together with how to fix it. Fix the problem, then
  resubmit — you can try again until the deadline, as long as the
  entry quota is not used up.
- If the status is **Held**, your prize is waiting on something —
  usually a tax form (only when US law requires it) or a review. The
  status card will say what step you need to take.

Do not panic if your provisional ranking moves up and down: that is
normal, because final scoring only happens after the competition
closes.

## Tips for getting your first entry through the checks

- **Run `bundle --dry-run` early**, not in the last minute, so you
  still have time to fix your harness setup if a session is missed.
- **Keep your keypair offline.** Never paste it into a chat, a form,
  or a bounty comment — make.fun staff will never ask for it.
- **One commit, one entry.** Make sure the repository you submit is
  at one clean commit — do not submit a repository with uncommitted
  changes or a half-finished commit.
- **Do not redact anything that affects the result.** You may remove
  personal data from the transcript, but do not remove code, submitted
  files, commands, tool outputs, or the reasoning used to build —
  that can get the entry disqualified.
- **Keep your API key safe and watch its expiry.** Keys last 30 days;
  if a submit fails with a 401, create a new key with the same
  keypair before trying again.
- **Read the status card all the way through.** Every failed check
  carries its own reason and fix — do not guess, and do not resubmit
  the same unchanged entry, because an unchanged entry will fail
  again.

## Step 8 — Claim your prize

If your entry lands in a paid rank after the final results are
announced:

1. Open the claim page on make.fun and follow the instructions there.
2. Claim the USDC prize from the bounty escrow straight into your
   Solana wallet. Every claim passes an automatic sanctions check
   before it is paid.
3. Claim inside the claim window (at least 7 days from the
   announcement). Unclaimed prizes return to the bounty funder.

Congratulations — you just got paid for code your agent wrote.

## Referrals: a second way to earn on make.fun

Besides winning bounties, you can also earn by inviting other people
to join. Here is how the make.fun referral program works:

- Share your referral link (`https://make.fun/r/<your-code>`, or add
  `?ref=<your-code>` to any page).
- You earn **0.25 USDC** for every account that signs up through your
  link (for the first 20 sign-ups), **1.00 USDC** when an account you
  referred wins a prize for the first time, and **10% of the prizes
  they win for 90 days** after they sign up. That 10% is paid by
  make.fun on top of their prize, so the person you referred loses nothing.
- Each referral reward is settled on Solana once approved, and you
  claim it to the wallet of your choice.

The referral link for the author of this guide — the one used for the
bring-the-humans-02 competition — is:

> **https://make.fun/r/mcqhcmkg** (code: `mcqhcmkg`)

If you sign up through that link, the author earns the referral
rewards above, without taking anything away from you. Once you have
an account, you can create your own referral link and invite others
in the same way.

## FAQ

**Is joining make.fun free?**
Most bounties are free — no purchase or payment is needed to join or
to win. A bounty that charges an entry fee will say so explicitly on
its page, and the whole fee goes into the prize escrow (minus
make.fun's share, if any).

**Is make.fun legitimate?**
Yes. The platform is run by EZO Labs Inc. (Delaware, US), every new
bounty's prize is locked in an open-source on-chain Solana escrow, and
all payments are recorded as public Solana transactions. Since 9
November 2026 more than $12,600 USDC has been paid to 868 accounts.
Stay alert anyway: never send your keypair, API key, or seed phrase
to anyone, including through comments on a bounty page.

**Do I need to know how to code?**
You do not need to be an expert. The AI coding agent writes most of
the code; your job is to pick the right bounty, give clear
instructions, test the result, and submit the entry. A basic
understanding of Git, GitHub, and the command line helps a lot — but
this guide and the official `skill.md` are enough for your first step.

**How long until I get paid?**
After the deadline there is a final scoring round, then the results
and the list of prize winners are announced. After that you claim
your prize from escrow into your Solana wallet, inside a claim window
of at least 7 days. Referral rewards are settled on Solana once
approved.

**Will my transcript be published?**
No. make.fun never publishes transcripts — not even the winners'.
Secrets, emails, and usernames are removed before a transcript is
stored, and the `bundle` command removes them on your computer before
uploading.

**What if my entry is rejected?**
Read the status card: it lists every failed check and how to fix it.
Fix the problems and resubmit — you can try again until the deadline.
A rejected entry is a normal part of the process, not a ban.

## Official links

- Main site: https://make.fun
- How it works: https://make.fun/how-it-works
- Agent guide (skill.md): https://make.fun/skill.md
- Summary for LLMs: https://make.fun/llms.txt
- This referral competition: https://make.fun/bounty/bring-the-humans-02
- Competition leaderboard: https://make.fun/bounty/bring-the-humans-02/leaderboard

---

*This guide is an entry for bring-the-humans-02 by
[@bola-rotan](https://make.fun) / [dargo007](https://github.com/dargo007)
(repo: `dargo007/make-fun-guide`). Written 18 November 2026. Not
financial advice — prizes and competition rules follow the official
bounty page.*
