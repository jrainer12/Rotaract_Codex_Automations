# Contributing

Thanks for wanting to add or improve a prompt. This repo is meant to stay small, practical, and easy for non-technical Rotary and Rotaract volunteers to use. Please keep that in mind when contributing.

## Repository conventions

- Every prompt lives in its own folder under `prompts/`.
- Folder names use lowercase kebab-case, e.g. `prompts/global-grant-application-filler/`.
- Each prompt folder contains:
  - `README.md` - the copy-paste prompt and a short explanation.
  - `sample-interaction.txt` - a made-up example run from start to finished output.
  - `sample-files/` - optional supporting files (templates, references) the prompt expects users to upload.

## Prompt structure

Every prompt should follow the same shape so users can switch between them without relearning anything. Inside the fenced ` ```text ` block, include:

1. A one-sentence role definition ("You are my ...").
2. A short statement of the job to be done.
3. A numbered, ordered workflow ("Work in this order: 1. ... 2. ...").
4. Section-by-section question lists so the AI does not ask everything at once.
5. Explicit rules (anti-hallucination, formatting, scope limits).
6. A defined output format.
7. A final "Begin now by ..." line so the AI starts the interaction itself.

Prompts should:

- Use plain, professional language.
- Tell the AI to label assumptions and avoid inventing facts.
- Include quality-control checks where applicable (e.g. "verify budget total equals funding total").
- Be tight enough that the output fits the intended downstream container (DOCX field, email, slide, etc.).

## Versioning

Each prompt is versioned by the date of its last meaningful change. Put a single line at the top of the fenced prompt block:

```text
Prompt version: YYYY-MM-DD
```

Update that date any time you change wording in a way that could affect output. Cosmetic edits to the surrounding `README.md` (typos, link fixes) do not require a version bump.

## Sample interactions

`sample-interaction.txt` should:

- Start with a disclaimer that names, places, costs, and details are fictional.
- Show the AI's first question, a realistic answer, and at least one full back-and-forth cycle.
- End at a point where the user can see what the finished output looks like.

Do not use real club, partner, beneficiary, donor, or grant data in samples.

## Adding a new prompt

1. Create `prompts/<your-prompt-name>/`.
2. Copy the template below into `README.md` and fill it in.
3. Add a `sample-interaction.txt` with a made-up example.
4. Add a bullet for the new prompt to the root `README.md` under "Prompts".
5. If your prompt needs a particular AI capability (file editing, web search, image input), add a row to the "AI Tool Compatibility" table in the root `README.md`.

### `README.md` template for a new prompt

````markdown
# <Prompt Title>

<One or two sentences describing what this prompt does and who it is for.>

Copy everything in the prompt below and paste it into <type of AI tool needed>. <Note any required capabilities such as DOCX read/write or web search.>

See `sample-interaction.txt` for a made-up example run.

```text
Prompt version: YYYY-MM-DD

You are my <role>.

Your job is to <one-sentence job description>.

Important: <one critical guardrail, if any>.

Work in this order:

1. <First step>
2. <Second step>
3. <Third step>

Start by asking me these setup questions:

- <Setup question 1>
- <Setup question 2>

After I answer, <describe next phase>.

Rules:

- <Rule 1>
- <Rule 2>
- <Rule 3>

Output format:

- <What the AI should return at the end>

Begin now by <first action the AI should take>.
```
````

## Pull requests

- Keep PRs focused on one prompt at a time when possible.
- In the PR description, say what behavior changed and why, and bump the `Prompt version` line if applicable.
- If you tested the prompt against a specific AI tool, mention which one in the PR description.
