# Elementum

Elementum is a React and Vite website built from a Figma design export and refined into a polished single-page experience. It includes the exported visual assets, responsive stage scaling, the Gerbil display font, and global styling for the final landing page.

## Tech Stack

- React 18
- Vite 6
- TypeScript
- Tailwind CSS 4
- Radix UI primitives
- Gerbil font loaded locally from `src/assets/fonts`

## Getting Started

Install dependencies:

```bash
npm install
```

Start the local development server:

```bash
npm run dev
```

Vite will print a local URL, usually:

```bash
http://127.0.0.1:5173/
```

Build for production:

```bash
npm run build
```

## Project Structure

```text
src/
  app/
    App.tsx                    # App shell and scaled website stage
    components/                # Reusable UI components
  assets/
    fonts/
      Gerbil-Regular.otf       # Local website font
  imports/
    Group355-1/                # Rendered Figma export and image assets
    Group355/                  # Alternate exported copy
  styles/
    fonts.css                  # Font-face declarations
    index.css                  # Global layout and responsive overrides
    theme.css                  # Theme tokens and global typography
  main.tsx                     # React entry point
```

## Styling Notes

The original design was exported as a fixed 1920px-wide canvas. The app wraps that export in a centered responsive stage so the website scales down cleanly on common screens while preserving the design composition.

Gerbil is applied globally through `src/styles/fonts.css` and `src/styles/theme.css`, including generated Figma text classes.

## Deployment

Any static hosting provider that supports Vite builds can serve this project.

Typical deployment command:

```bash
npm run build
```

Publish the generated `dist/` directory.

## Repository

GitHub: https://github.com/Aslamak05/Elementum
