---
name: @xlearnmore-coding-skill
description: "GitHub profile skill from @xlearnmore. Use it when the task would benefit from mimicking this developer's repo choices, coding style, and implementation techniques."
---

## What they tend to build

- Small, practical utilities rather than large platforms. The clearest repo is a **Windows Forms desktop tool** for converting images to WebP.
- Feature sets are straightforward and task-driven: **select files/folders, batch process, adjust a quality setting, choose an output directory, show progress, handle errors**.
- Their profile README suggests a broad but pragmatic interest in **backend work** plus learning **C++**, so expect utility-first code over ornamental abstractions.

## Coding patterns to mirror

- Prefer **simple event-driven flows**: user clicks a button, selects input, adjusts a setting, runs an action, sees live status.
- Keep operations **explicit and incremental**:
  - validate inputs early
  - process multiple items in a loop
  - update progress/status after each item
  - surface failures per-file instead of failing the whole batch
- Use **clear, descriptive names** for UI actions and settings. Their README language is very literal: “Select Images”, “Select Folder”, “Convert to WebP”, “Output Folder”.
- Favor **practical error handling** and user feedback over silent failure.
- In docs and UI text, they tend to use **short feature bullets** and direct instructions, often with emojis for readability.

## Product and UI taste

- Strong preference for **utility UI**: uncluttered Windows desktop interfaces that reduce steps to the core workflow.
- The README emphasizes **discoverability** through labeled buttons, default values, progress tracking, and live status updates.
- Visual presentation leans friendly and approachable:
  - emoji-enhanced headings and bullets
  - checkmarks/arrows for feature lists
  - “how to use” sections with step-by-step flows
- Expect UI decisions that prioritize **speed of use** over deep customization.

## Tech stack clues

- Most concrete signal: **C# + Windows Forms + .NET Framework 4.7.2+**.
- Image conversion uses **FreeImageAPI / FreeImage.dll**.
- The profile README lists familiarity or interest in:
  - **C++**
  - **PHP / Laravel**
  - **MySQL / MS SQL Server**
  - **HTML / Bootstrap / Tailwind**
  - **Git, Nginx, Azure, Google Cloud, Figma**
- That mix suggests comfort moving between **desktop tooling, backend services, and lightweight web stacks**, but the strongest repo evidence is still desktop C#.

## When to inspect repos first

- If you’re adding anything involving:
  - **Windows Forms layout or event handlers**
  - **batch file processing**
  - **image conversion / file dialogs / output path handling**
  - **progress bars, status labels, or per-item error reporting**
- Inspect first if you need to match their exact conventions for:
  - control naming
  - how they structure helper methods
  - whether logic lives in form code-behind or separate classes
  - how they integrate external DLLs like FreeImage
- Also inspect before making docs or UI copy, since their public-facing style is **very specific, emoji-heavy, and feature-led**.

## Repo Map

- [xlearnmore/WebPConverterGUI](https://github.com/xlearnmore/WebPConverterGUI): A Windows Forms application that allows users to convert images (JPG, PNG, BMP, GIF) to WebP format using the FreeImageAPI. (2 stars, C#)
- [xlearnmore/xlearnmore](https://github.com/xlearnmore/xlearnmore): Hello world!, this is my profile (1 stars)

## How To Use This Skill

- Reach for this skill when the user asks for Xlearnmore's style, when the repo stack matches this person's ecosystem, or when studying their real code would reduce made-up output.
- Pick one or more relevant repositories from the list above based on the current task.
- Clone the most relevant repository or repositories into `/tmp` for temporary inspection.
- Study the implementation details, naming patterns, architecture, UI taste, and tooling choices there.
- Return to the main task and apply the useful patterns you observed instead of copying blindly.
- Treat the upstream repositories as reference material for style and technique, then adapt them to the current codebase responsibly.
