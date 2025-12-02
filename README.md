# 2025-12-RNS-SoC-Talk

A reveal.js presentation for Returning NSMen Talk at NUS School of Computing.

## Prerequisites

- [Node.js](https://nodejs.org/) (v14 or higher recommended)
- npm (comes with Node.js)

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/laurenceputra/2025-12-RNS-SoC-Talk.git
   cd 2025-12-RNS-SoC-Talk
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

## GitHub Pages Hosting

This repository includes only the necessary reveal.js files in the `vendor/` directory to support hosting the presentation directly on GitHub Pages without a build step. The required CSS and JavaScript files are bundled in the repository so that `index.html` can reference them directly via relative paths.

To host on GitHub Pages:
1. Enable GitHub Pages in your repository settings
2. Set the source to the branch containing this code
3. The presentation will be available at `https://<username>.github.io/2025-12-RNS-SoC-Talk/`

## Usage

### Running the Presentation

Start a local server to view the presentation:

```bash
npm start
```

Then open your browser and navigate to `http://localhost:3000`.

Alternatively, you can simply open `index.html` directly in your browser, though some features may require a local server.

### Keyboard Controls

- **Arrow keys** or **Space**: Navigate between slides
- **Esc** or **O**: Overview mode
- **S**: Speaker notes (if enabled)
- **F**: Fullscreen mode

## Presentation Outline

1. **My SoC and Career Journey** - Education and career path
2. **What I Learned at SoC** - Technical and soft skills that benefited my career
3. **Notable Past Projects** - Shareable projects and achievements
4. **Industry Insights & Trends** - Emerging technologies and industry shifts
5. **Tips & Advice for Freshmen** - Academic, career, and personal development tips

## Customization

### Changing the Theme

To change the presentation theme, modify the theme CSS link in `index.html`:

```html
<link rel="stylesheet" href="vendor/reveal.js/dist/theme/black.css">
```

Available themes include: `black`, `white`, `league`, `beige`, `sky`, `night`, `serif`, `simple`, `solarized`, `blood`, `moon`.

### Adding Speaker Notes

Add speaker notes to any slide using the `<aside class="notes">` element:

```html
<section>
  <h2>Slide Title</h2>
  <aside class="notes">
    Speaker notes go here...
  </aside>
</section>
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Built With

- [reveal.js](https://revealjs.com/) - The HTML Presentation Framework
