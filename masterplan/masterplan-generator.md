# Masterplan Core

Four sections of the Masterplan Generator, in order: Ground Rules, Project Brief, Architecture, Task Plan.

Label key: RULE: add it to masterplan.md as written; follow it during the build, not now. DRAFT: write that part of masterplan.md, then show me for review. USER INPUT: ask me first, then write my answer into masterplan.md.

## 1. Ground Rules: how we work

RULE: Build from masterplan.md, idea.md and my screenshot; borrow language, tools, specs, or open-source code from examples as I choose.

RULE: At the start of the build, check tools, libraries, GitHub login, that this folder is its own repo root, and that each data source's host and port can be reached, on my platforms; show pass/fail.

RULE: After each change, measure the app against the Project Brief's screen list; show pass/fail.

RULE: After each working step: run all tests, show me proof, commit, and push to GitHub. Keep going within a stage; stop only at stage end, on a failed test, after two failed fixes, or for my decision.

RULE: When code and masterplan disagree, propose only major changes, one line each; update the masterplan after I approve.

## 2. Project Brief: what the app does

DRAFT: Summarize what my app does in a few sentences, from idea.md, my screenshot, and any example app.

DRAFT: From my screenshot, list screen elements and controls, with where each sits.

DRAFT: For each feature in idea.md, describe what the user does and sees, with testable ranges where possible.

DRAFT: List where my app's data comes from, and how we'll check each source works, including after a reconnect. Send every server setting on each connect; never rely on settings from earlier sessions.

USER INPUT: Ask which features from idea.md my app must do this iteration, and which wait; suggest if I'm unsure.

## 3. Architecture: what it's built with

USER INPUT: Recommend a language and tools, Python unless my example suggests better; explain each and let me choose.

DRAFT: List what must be installed on each platform in idea.md, and how to check each works.

RULE: Keep the app responsive while it works, never stuck waiting on data or input.

DRAFT: Propose a handful of well-structured modules, one line each, each testable on its own.

RULE: Keep a short list of known limitations in the masterplan; update it as we go.

## 4. Task Plan: in what order

DRAFT: Break the build into about 5 stages: environment (including measuring my screenshot with a script), data connections tested on live servers and ending with a bare window showing live data, core logic, features, and UI. Give each stage sub-steps and one done-when line.

DRAFT: For each sub-step, say how we'll test it and what result means it works.

RULE: Test connections to outside data with real servers before building screens that depend on them.

RULE: Get a simple version running early, then add features one at a time, testing each.

DRAFT: Add a final step: review what went wrong and propose masterplan updates for my approval.
