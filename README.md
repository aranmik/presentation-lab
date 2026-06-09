# Presentation Lab

Project Signal Personal presentation lab.

presentation-lab is a separate visual experiment workspace for battle readability, avatars, action lines, attack/hit/heal presentation, speed gauges, skill labels, combat log readability, status marks, and front/back row expression.

## Purpose

This lab exists to test presentation ideas before anything is added to the main game.

The goal is not to make a pretty standalone page first. The goal is to make combat roles, actions, targets, and results easier to read on a 390px mobile screen.

## Relationship To The Main Game

- `project-signal-personal` is the main game.
- `presentation-lab` is an experiment lab, not the main game.
- Luda works here as presentation experiment lead.
- Yuki judges direction and decides whether an experiment is ready to be summarized for porting.
- Naranim checks the result by eye and makes the final choice.
- Ren owns main game implementation and ports approved ideas into `project-signal-personal`.

## Main Game Safety Rule

Luda does not directly modify `project-signal-personal` from this lab.

Even if an experiment looks good, it stays in `presentation-lab` until Yuki and Naranim approve it for main game use.

Before main game porting, the experiment result should be summarized clearly for Yuki and Ren.

## Preview Workflow

The lab can be checked through the Codex Browser / Preview panel.

Current local preview server:

```text
http://localhost:4177/avatar-prototype
```

Fixed current preview page:

```text
http://localhost:4177/preview.html
```

Use `preview.html` as the right-side Browser / Preview page when Naranim wants to keep one fixed tab open. Luda updates this page to point at the current experiment.

Recommended flow:

1. Luda updates a lab file.
2. Naranim checks the local preview in the right Browser / Preview panel.
3. If the idea feels good, Luda summarizes the experiment result.
4. Yuki decides whether and how it should be moved toward the main game.
5. Ren ports approved ideas into `project-signal-personal`.

## Current Prototype

`avatar-prototype.html` is Avatar Prototype 01.

Current state:

- Warrior: sturdy front row, sword and shield, stable stance.
- Priest: back row support, staff, healing aura.
- Archer: back row attack, bow, agile stance.

Prototype goal:

- Readable inside compact mobile battle cards.
- Class identity should come from silhouette, parts, stance, and motion direction, not only color.
- Future main game use should be possible inside a `unit-card`-sized space, after Yuki and Naranim approve and Ren ports it.

## Next Experiment Candidates

Current suggested priority:

1. Avatar Prototype 01 readability polish.
2. Action Line Prototype 01: small attack, heal, and hit feedback readability test.
3. Battlefield Layout Prototype 01: party slots, enemy footprint, boss presence, and quiet FX path sketch.
4. Speed gauge or action-ready state prototype.
5. Skill label and combat log readability prototype.
