# Copilot Instructions for 2025-12-RNS-SoC-Talk

## Project Overview

This repository contains a reveal.js presentation for the Returning NSMen Talk at NUS School of Computing (December 2025). The presentation covers career journeys, skills learned at SoC, notable projects, industry insights, and advice for freshmen.

## Tech Stack

- **Presentation Framework**: reveal.js v5.2.1
- **Languages**: HTML, JavaScript, CSS
- **Runtime**: Node.js (v14 or higher)
- **Package Manager**: npm
- **Development Server**: serve

## Project Structure

```
├── index.html          # Main presentation file containing all slides
├── package.json        # Node.js dependencies and scripts
├── package-lock.json   # Locked dependency versions
├── README.md           # Project documentation
├── LICENSE             # MIT License
└── .gitignore          # Git ignore patterns
```

## Development Guidelines

### Running the Presentation

1. Install dependencies: `npm install`
2. Start the development server: `npm start`
3. Open `http://localhost:3000` in your browser

### Working with Slides

- All slides are defined in `index.html` within the `<div class="slides">` container
- Each `<section>` element represents a slide
- Nested `<section>` elements create vertical slide stacks
- Use `<aside class="notes">` for speaker notes

### Reveal.js Features

- Available themes: black, white, league, beige, sky, night, serif, simple, solarized, blood, moon
- Enabled plugins: Markdown, Highlight (code syntax), Notes
- Navigation: Arrow keys, Space, Esc (overview), S (speaker notes), F (fullscreen)

## Coding Conventions

- Use semantic HTML elements
- Maintain consistent indentation (2 spaces)
- Keep slide content concise and readable
- Add comments for slide sections using HTML comments (`<!-- -->`)
- Follow existing patterns when adding new slides

## Testing

This project uses `npm test` which currently returns success without running specific tests.

## Additional Resources

- [reveal.js Documentation](https://revealjs.com/)
- [reveal.js GitHub Repository](https://github.com/hakimel/reveal.js)

## Copilot Agent Workflow (Slides Editor & Reviewer)

This repo includes two GitHub Copilot agent instruction files under `.github/` that you can use as role-specific prompts for editing and reviewing slide content.

- `.github/slide-editor-agent.md` — instructions for the Slides Editor Agent (edit slides directly in `index.html`, add notes, keep bullets concise, inject light humor when appropriate).
- `.github/slide-reviewer-agent.md` — instructions for the Slides Reviewer Agent (industry-focused reviewer that checks tone, accuracy, clarity, and inclusive humor).

How to trigger these agents via Copilot:
1. Open `index.html` and the relevant slide `<section>` you want to update.
2. Open your GitHub Copilot chat or in-editor prompt and include a short trigger line followed by the role file path. Example prompts:
	- "Act as the Slides Editor Agent — follow `.github/slide-editor-agent.md` and propose a revised slide for `index.html` section with id='<your-id>'"
	- "Act as the Slides Reviewer Agent — follow `.github/slide-reviewer-agent.md` and review this PR or the `index.html` diff; provide inline suggested edits"
3. Follow the advice and suggested edits from Copilot; apply them to `index.html` and add `aside class='notes'` speaker guidance where helpful.

Notes & Conventions
- Use `slides:` prefix in commit messages for content changes (e.g., `slides: add 'Interview Prep Tips' slide`) and `chore:` for script/structure changes.
- Keep humor concise: 1–2 short lines maximum, preferably held in notes rather than slide headlines.
- If changes are structural (e.g., adding insertion markers or modifying scripts), split these into a separate PR and reference both PRs.
- Reviewers should prefer the `index.html` single-source editing approach instead of editing generated content elsewhere (like `data/`), unless a generator is explicitly added.

This workflow keeps Copilot usage within the native Copilot instruction context and avoids third-party automation for content generation. Use the two role files as the definitive guides for behavior and tone when prompting Copilot.
