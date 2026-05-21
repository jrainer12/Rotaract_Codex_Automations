# Rotaract Codex Automations

This repository stores copy-paste prompts for AI tools.

Each prompt lives in its own folder with a `README.md`. Open the folder for the task you want, copy the prompt, paste it into your AI tool, and follow the questions it asks.

## Prompts

- [Global Grant Application Filler](./prompts/global-grant-application-filler/) - interviews you for a Rotary Global Grant application, fills the template, and returns a completed file.
- [Global Grant Application Completeness Check](./prompts/global-grant-application-completeness-check/) - reviews a filled Rotary Global Grant application and reports missing, weak, or inconsistent items before submission.
- [Service Project Finder](./prompts/service-project-finder/) - researches local needs and recommends realistic Rotary or Rotaract service project ideas that fit budget, volunteers, partners, and timeline.

## AI Tool Compatibility

These prompts are written to work with any general-purpose chat AI. They have been tested most thoroughly on OpenAI models (for example, ChatGPT). Other models such as Claude or Gemini should also work, but results may vary.

Different prompts need different AI capabilities:

| Prompt | Needs |
| --- | --- |
| Global Grant Application Filler | An AI tool that can read uploaded DOCX files and return a filled DOCX file. |
| Global Grant Application Completeness Check | An AI tool that can read uploaded DOCX files. |
| Service Project Finder | An AI tool that can search the web. |

Pick a chat tool that supports what the prompt needs. If your tool cannot return a DOCX file, the filler prompt will still produce application text you can paste into the template yourself.

## Folder Structure

Each prompt folder can include:

- `README.md` - the copy-paste prompt.
- `sample-interaction.txt` - a made-up example conversation from start to finished output.
- `sample-files/` - optional files to upload with the prompt.

## How to Use

1. Open a prompt folder.
2. Copy the full prompt from its `README.md`.
3. Check `sample-interaction.txt` if you want to see what answers might look like.
4. Paste the prompt into an AI tool that supports what the prompt needs (see the compatibility table above).
5. Upload any requested template or source files when the prompt asks for them.
6. Answer the AI tool's questions until it can produce the finished output.

## Contributing

See [CONTRIBUTING.md](./CONTRIBUTING.md) for the prompt template, folder conventions, and versioning rules.

## License

MIT - see [LICENSE](./LICENSE).
