# Room concept image handoff

This folder contains everything needed to generate the nine room concepts on another computer. It does not contain an API key, account identifier, family information, inspection notes or generated images.

## Files

- `manifest.json` is the source of truth for room names, source photos, final filenames, plans and complete prompts.
- `prompts.md` is the human-readable generation and review guide.
- `generated/` is where final concept images belong.
- `../new-room-ideas.html` reads the manifest and automatically shows a concept when its expected WebP or PNG file is present.

## Recommended Codex workflow

1. Clone or pull this repository on the image-capable laptop.
2. Open the repository in a Codex session where image generation is available.
3. Ask Codex to read this file, `prompts.md` and `manifest.json`.
4. Work on one room at a time. Give the listed source photo to the image tool as **Image 1: edit target**, then use that room's complete `prompt` value.
5. Inspect the result against the checklist in `prompts.md`. Make only one targeted correction at a time and repeat every preservation constraint during edits.
6. Save the accepted image to the room's exact `output` path. A PNG using `fallbackOutput` also works.
7. Preview `../new-room-ideas.html`, then commit and push only the accepted room images.

Suggested instruction to paste into the new Codex session:

> Read `room-ideas/README.md`, `room-ideas/prompts.md` and `room-ideas/manifest.json`. Generate one room concept at a time. Treat each listed source photo as the edit target, preserve every architectural invariant, review the output against the privacy and safety checks, and save the accepted result under the exact output filename. Do not add or expose credentials.

The built-in image workflow does not need a repository key. If image generation is not available in that Codex session, stop rather than adding a secret to this public repository. An optional API-backed workflow must be configured privately on that computer; never paste a key into chat, HTML, Markdown, JSON, JavaScript, Git history or a screenshot.

## Output conversion

The page prefers WebP and falls back to PNG. If a tool returns PNG and ImageMagick is available, make a metadata-stripped WebP copy:

```sh
magick accepted-image.png -strip -quality 88 room-ideas/generated/family-room-concept.webp
```

Replace the final filename with the `output` value for that room. Keep the source aspect ratio. Do not stretch the room or crop away doors, windows, ceiling concerns or exit paths.

## Local preview

From the repository root:

```sh
python3 -m http.server 4173
```

Then open `http://127.0.0.1:4173/new-room-ideas.html`. A missing output correctly appears as **Concept image pending**.

## Commit safety

Before pushing, confirm that only intended room concepts and source changes are staged:

```sh
git status --short
git diff --cached --stat
git diff --cached
```

Do not commit `.env` files, credentials, private inspection photos, exported browser backups, personal notes, financial documents, names, phone numbers, email addresses or readable family material.
