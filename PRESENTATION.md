# Presentation Guide

Short notes for presenting this repo to a Rotary, Rotaract, or club-leadership audience. Plan on roughly 10-15 minutes including the walkthrough demo. Adjust depth based on the audience.

## Before you start

- Open the repo in a browser tab at the root `README.md`.
- Open the pre-recorded ChatGPT walkthrough in a second tab: <https://chatgpt.com/share/6a0e695d-6c44-83ea-ad12-f5a0300c2cfe>
- Optional: open `prompts/global-grant-application-filler/sample-interaction.txt` in a third tab as a backup if the share link is slow or unreachable.
- Test both links on the actual presentation network before you start. Public Wi-Fi sometimes blocks `chatgpt.com`.

## The hook (~1 minute)

- Clubs spend hundreds of volunteer hours every year on the same recurring tasks: grants, project scoping, donor outreach, event planning, newsletters, reports.
- Most members already know AI tools could help, and most have tried opening ChatGPT and typing a sentence. The results are usually generic, inconsistent, or quietly wrong - because a one-sentence prompt cannot carry Rotary terminology, required sections, or quality bars.
- This repo flips that around. Instead of every member learning to prompt well, we write the prompt once - carefully, with guardrails and quality checks - and everyone copies and pastes it.

## What it is (~1 minute)

- A growing library of curated AI prompts for Rotary, Rotaract, and club work. Anyone can copy a prompt, paste it into a chat AI, and get usable output without knowing how to prompt.
- It started with Rotary Global Grant work because grants are one of the most painful, repetitive tasks many clubs face. But the approach applies anywhere a task is recurring and has a predictable shape: membership outreach, event planning, communications, fundraising, district reporting, partnership emails, board materials.
- The three prompts available today are examples, not the point:
  - **Global Grant Application Filler** - interviews you and fills the actual Rotary template.
  - **Global Grant Application Completeness Check** - reviews a filled application before submission.
  - **Service Project Finder** - researches local needs and proposes realistic project ideas.
- Not code, not a website, not a paid service. Just text you copy. Anyone can use it with no setup.

## The core idea (~1 minute)

This is the slide-worthy idea if you only have one. Put it up explicitly.

- A one-sentence prompt to ChatGPT is like asking a brand-new volunteer to write a grant in one sitting with no template and no rules.
- A curated prompt is like handing them a checklist, the template, the terminology, and a senior reviewer who refuses to skip steps. Same AI, very different output.
- We do not need every Rotarian to learn prompt engineering. We need a small number of well-engineered prompts that any Rotarian can copy.

## Demo (~5-8 minutes)

Walk the audience through the pre-recorded ChatGPT chat instead of running anything live. This avoids stalls, hallucinations, and slow interviews.

1. Open the root `README.md`. Point out the **AI Tool Compatibility** table so people understand not every tool works for every prompt.
2. Click into `prompts/global-grant-application-filler/`. Briefly show the `README.md` so the audience sees the structure of the prompt: role definition, ordered workflow, section-by-section questions, quality-control rules, text-only fallback.
3. Switch to the pre-recorded ChatGPT chat: <https://chatgpt.com/share/6a0e695d-6c44-83ea-ad12-f5a0300c2cfe>
4. Scroll through the conversation slowly. Pause on:
   - The opening setup questions (how the prompt structures the interview).
   - One or two section-by-section question groups (so people see it does not dump everything at once).
   - The final filled output (the headline payoff).
5. After the walkthrough, briefly mention the other two prompts and point at their `sample-interaction.txt` files so the audience knows they exist without sitting through another full demo.

## Talking points (pull in as needed)

- "Two members opening ChatGPT and typing 'help me with our grant' will get two different answers. Two members copying the same prompt from this repo will get the same structure, the same questions, and the same guardrails."
- "Each prompt is opinionated on purpose. It tells the AI what order to ask questions in, what it must not hallucinate, and exactly what format to return."
- "Curated prompts raise the floor for new AI users and raise the ceiling for experienced ones. Even people who are good at prompting forget to add guardrails and quality checks. The prompt does it for them."
- "We version every prompt by date. The version line at the top tells users which version they pasted, so changes are traceable."
- "There is a contribution guide and a pull request template. Any member who wants to add or improve a prompt has a clear path. The Grant Filler is just the first example - the bigger play is the library."
- "It is MIT licensed. Any other club, district, or Rotaract group can fork it, adapt it, and use it. Sharing is encouraged."
- "The Grant Filler has a text-only fallback mode for tools that cannot return DOCX, so nobody gets stuck."

## Anticipated questions

- **Why not just use ChatGPT directly?** You can, for one-off or exploratory work. For recurring tasks with structure, terminology, and quality bars - grants, reports, donor outreach - a curated prompt produces consistent, guardrailed output that an ad-hoc chat does not. Two members asking ChatGPT the same question on the same day get different answers; two members pasting the same prompt from this repo get the same structure.
- **Why is the repo so grant-focused right now?** Grants happened to be the first painful task we tackled. The repo is a general library and is expected to grow into membership outreach, event planning, communications, fundraising, district reporting, and other recurring club work.
- **Does this replace the Grant Center?** No. The Filler produces a draft. Final review and submission still happen in Rotary's Grant Center.
- **Will the AI invent facts?** The prompts explicitly forbid invented facts and require the AI to label assumptions. Always verify before submitting anything.
- **Which AI tool should we use?** Tested most on OpenAI models. Claude and Gemini should also work, but results may vary. Check the compatibility table.
- **What if our AI tool cannot return a DOCX?** The Filler prompt has a built-in text-only fallback that produces pasteable output organized by section.
- **Is our data safe?** Treat any AI chat tool the way you would treat email to a vendor. Avoid real personal data in samples. The repo itself stores no club data.
- **Can we add our own prompts?** Yes - see [CONTRIBUTING.md](./CONTRIBUTING.md) for the folder structure, prompt template, and versioning rules.

## Call to action

- Try one prompt this week, even on a small task.
- If a prompt gets something wrong, open an issue or send feedback so we can improve it - the whole point is that fixes compound across clubs.
- If your club has a recurring task that an AI could handle with the right instructions, propose a new prompt. The grant prompts are just the start.

## Working session: pick our next prompts

Mention this near the end of the talk so people know the conversation continues. Block off 30-60 minutes right after, while the energy is still up.

### What makes a good candidate for a curated prompt

A task earns a curated prompt when most of these are true:

- It is recurring (we do it more than once a year, often more than once a month).
- It follows a predictable shape (the same sections, fields, or beats every time).
- It has hidden quality bars (Rotary terminology, required sections, math that must reconcile).
- Members currently do it differently every time, with inconsistent quality.
- Skipping a step or missing a section has real consequences (rejected grant, lost donor, no-show event).

If a task is one-off, exploratory, or already so simple that a sentence to ChatGPT works fine, it probably does not need a curated prompt.

### Starter idea list

Bring this list into the working session. Cross off anything we already have. Add what the room shouts out.

**Membership**

- New member onboarding interview
- Lapsed member re-engagement message
- Prospective member outreach
- Annual membership survey designer
- Member retention check-in script

**Communications**

- Newsletter section drafter
- Social media post pack (multi-platform)
- Announcement and press release drafter
- Annual report president's letter
- Email signature and template generator

**Fundraising**

- Donor solicitation letter
- Gift acknowledgment letter (by tier)
- Pledge follow-up sequence
- Year-end giving appeal
- Capital campaign case statement

**Events**

- Run-of-show timeline generator
- Sponsor pitch and sponsorship deck drafter
- Post-event recap and thank-you generator
- Event budget builder
- Speaker invitation letter

**Volunteers and partners**

- Project role description drafter
- Volunteer training brief
- Cold outreach email to a nonprofit, school, or vendor
- MOU drafting helper
- Partner check-in agenda

**Board and reporting**

- Board agenda drafter from topics
- Minutes cleanup and summarizer
- Briefing note for a board decision
- President's monthly report
- Year-end impact report

**Rotary-specific**

- District grant application helper (smaller than global grant)
- District grant report drafter
- Polio Plus campaign messaging
- Youth Exchange host family prep
- RYLA application reviewer
- Rotary Peace Fellow application helper

### How to run the working session (45 minutes)

1. **5 min - frame the goal.** "We will leave with at least two new prompts in flight." Restate the criteria above so the room scopes ideas correctly.
2. **10 min - generate.** Everyone calls out tasks they find painful or repetitive. Capture on a whiteboard or shared doc. Encourage specificity ("monthly board agenda," not "stuff for meetings").
3. **5 min - cluster and score.** Group similar ideas. Mark each one with a quick score: pain (1-5), frequency (1-5), AI-suitability (1-5). Total = priority.
4. **5 min - pick the top two or three.** Dot-vote if the room is split.
5. **15 min - rough out one prompt together.** For the highest-priority idea, draft:
   - The role (one sentence).
   - The ordered workflow (3-5 steps).
   - The setup questions to ask the user.
   - The expected output format.
6. **5 min - assign owners and next steps.** Each picked idea gets a named owner who will open a PR using the template in `CONTRIBUTING.md`. Set a date for the next check-in.

Leave the session with named owners, not just ideas. An idea without an owner is a wish list.

## If the demo breaks

- The share link will not load (network block, expired share, ChatGPT down): switch to `prompts/global-grant-application-filler/sample-interaction.txt` in the repo and walk through it the same way. The content mirrors the shared chat.
- The repo will not load (network issue): you should already have it cloned locally. Open the files in your editor and present from there.
- Someone asks "but does this actually work live?": offer to run the Service Project Finder afterward as a side conversation. Do not switch the talk into a live demo on the fly.
- Time runs short: skip step 4's scroll-through and jump straight to the final filled output in the shared chat. The payoff is the strongest single moment of the demo.
