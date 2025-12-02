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
