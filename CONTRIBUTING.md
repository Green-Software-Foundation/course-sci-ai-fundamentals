# Contributing to SCI for AI Fundamentals

Thank you for your interest in contributing to this course. This repository stores the content assets for the SCI for AI Fundamentals course produced by the Green Software Foundation.

## What Lives Here

| Folder | Contents |
|--------|---------|
| `modules/` | Per-module descriptions, video links, and scripts |
| `assessment/` | Quiz questions and digital badge information |
| `assets/` | Shared brand assets, images, LMS visuals, and templates |
| `course-outline.md` | Full course outline |

## How to Contribute

### Reporting issues

If you find an error in a script, incorrect information in a module description, or a broken link, please [open a GitHub issue](../../issues) with:

- The file path and line number
- What the current content says
- What it should say, with a source or rationale

### Updating a video script

1. Fork the repository and create a branch from `main`
2. Edit the relevant script file in `modules/<module-name>/scripts/`
3. Follow the script format defined in [`assets/templates/script-template.md`](assets/templates/script-template.md)
4. Open a pull request with a clear description of the change

### Updating module content

Module descriptions and learning outcomes live in each module's `README.md`. These should reflect the SCI for AI specification and the filmed video content. If you propose changes that affect the course structure, please open an issue first to discuss.

### Adding or replacing visual assets

- Module-specific visuals go in `modules/<module-name>/assets/`
- Shared visuals (used across modules or on the LMS) go in `assets/images/` or `assets/lms/`
- Brand assets (logos, colour palette, typography) go in `assets/brand/`
- Preferred formats: SVG for diagrams, PNG for raster images, MP4 for video (link externally rather than committing)

### Adding video links

Videos are hosted externally (e.g. YouTube or Vimeo). Update the `videos.md` file in the relevant module folder with the hosted URL, title, and duration. Do not commit video files to this repository.

## Style Guidelines

- Write in plain, direct English
- Use sentence case for headings
- Follow the structure of existing module READMEs (see [`assets/templates/module-readme-template.md`](assets/templates/module-readme-template.md))
- Scripts should be written as they would be spoken aloud — conversational, not academic

## Licence

By contributing, you agree that your contributions will be licensed under [Creative Commons Attribution 4.0 International](LICENCE.md).
