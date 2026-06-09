# Presentation Rules

## Core Principle

Readability comes before prettiness.

A good experiment makes the battle flow, role, target, action, and result easier to understand on a small mobile screen.

## Main Game Boundary

- Do not modify `project-signal-personal` from this lab.
- Do not port experiments directly into the main game.
- Do not copy main game code into the lab.
- Do not copy R&D code into the lab.
- If an experiment is selected, summarize it first.
- Yuki and Naranim decide whether it is worth porting.
- Ren implements approved ideas in the main game.

## Visual Direction

- Prioritize combat flow and class readability.
- Check the 390px mobile view first.
- Do not judge by a zoomed PC screen first.
- Avatar size should assume future placement inside a compact `unit-card`.
- Do not rely only on color changes.
- Separate classes through silhouette, parts, stance, and motion.
- Prefer clear role language: front row holder, back row healer, back row attacker.

## Technical Rules

- No image files.
- No external libraries.
- No canvas.
- No npm structure.
- No build tools.
- Use plain HTML/CSS first.
- Use JavaScript only when needed, and keep it minimal.
- Keep experiments easy to open as plain local HTML.

## Naming Rules

Use `lab-` or `proto-` prefixes for experiment class names to reduce collision risk with the main game.

Examples:

- `lab-page`
- `lab-stage`
- `lab-summary`
- `proto-avatar`
- `proto-part`
- `proto-warrior`

Avoid reusing main game class names directly unless the experiment is explicitly about testing a future mapping.

## Preview Rules

- Preview through the Codex Browser / Preview panel when possible.
- Use the local server URL for active checks.
- Current Avatar Prototype 01 URL:

```text
http://localhost:4177/avatar-prototype
```

- When judging a prototype, check whether the role is readable before checking whether it is pretty.
- If a detail only works on a large PC view, treat it as unproven until it works at 390px.

## Scope Rules

Keep each lab step small.

Allowed lab targets:

- Character avatar readability.
- Action lines.
- Attack, hit, and heal presentation.
- Speed gauge or action-ready state.
- Skill labels.
- Combat log readability.
- Status marks.
- Front/back row expression.

Do not jump to 24 classes, large animation systems, or full main game UI reconstruction unless Yuki and Naranim explicitly approve that scope.
