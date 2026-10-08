# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## What this repo is

Learning notes and example code for the "Chai aur Code" JavaScript (Hindi) YouTube series.
It is not an application: there is no `package.json`, no dependencies, no build, no linter, and no test suite.
Each file is a standalone lesson snippet that demonstrates one concept, mostly via `console.log` / `console.table` output.

## Running code

- Plain `.js` files run directly with Node (the devcontainer uses Node 18): `node 01_basics/01_variables.js`
- `.html` files (DOM, events, fetch/API, `bind`, closures) are meant to be opened in a browser.
  `.vscode/settings.json` configures the VS Code Live Server extension on port 5501.
- There are no tests; "verifying" a change means running the file and checking console output.

## Layout

Folders are numbered in the order the course teaches them, and each builds on the previous:

- `01_basics` - `03_basics`: variables, data types, conversion, comparison, strings, numbers/math, dates, arrays, objects, functions, scope, arrow functions, IIFE
- `04_control_flow`, `05_iterations`: conditionals, truthiness, switch, loops, and array higher-order functions
- `06_dom`, `08_events`: browser-only HTML pages with inline `<script>` tags
- `07_projects/projectsset1.md`: solution code for the DOM projects hosted on StackBlitz (https://stackblitz.com/edit/dom-project-chaiaurcode?file=index.html)
- `09_advance_one`: promises, async/await, fetch, XHR API requests
- `10_classes_and_oop`: object literals, prototypes, `call`/`bind`, classes, inheritance, static props, getters/setters (`notes.md` has written notes)
- `11_fun_with_js`: closures

## Conventions

- Code intentionally contains commented-out lines, deliberate errors, and explanatory comments showing what is "not allowed" - these are teaching material, not bugs to clean up.
- Keep new lessons consistent with the existing style: one concept per file inside the matching numbered topic folder, explained through console output and inline comments.
