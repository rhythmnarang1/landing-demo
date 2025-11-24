# Reflection on Intentional Merge Conflict — landing-demo

## Project summary
This repository contains a simple landing page (`index.html`, `styles.css`, `script.js`). The aim was to demonstrate branching, merging, intentionally creating a merge conflict, and resolving it locally using VS Code and Git.

## What caused the conflict
Both branches edited the exact same line in `index.html` — the hero `<p id="hero">` line. Since `feature-header` and `feature-hero` changed that same line to different texts, Git could not automatically decide which change to keep when merging `feature-hero` into a `main` that already contained `feature-header`.

## Exact steps taken to resolve
1. `git checkout main` and `git pull origin main` to ensure main was current.
2. `git merge feature-hero` — caused conflict in `index.html`.
3. `git status` — confirmed `both modified: index.html`.
4. Opened the project in VS Code; inspected conflict markers `<<<<<<<`, `=======`, `>>>>>>>`.
5. Used VS Code merge controls to **Accept Both Changes**, then manually edited the result to a combined, coherent hero text:
<p id="hero">Combined: A dazzling, best-in-class hero message — edits from feature-header & feature-hero combined.</p> ```
6. `git add index.html` 
7. `git commit -m "Resolve merge conflict in index.html — combine feature-header & feature-hero"` 
8. `git push origin main` 
9. Collected screenshots in `evidence/` showing each stage.

## Learnings

Merge conflicts are expected when multiple developers change the same lines. They’re not an error — they require intentional human resolution.
git status and inspecting files are primary tools for identifying and fixing conflicts.
VS Code provides a friendly UI for resolving conflicts (accept current, incoming, or both).
Frequent small merges and communication reduce painful conflicts; however, learning to resolve them is essential for collaboration.


##Artifacts

index.html — final merged file
styles.css, script.js — supporting files
evidence/ — screenshots of conflict and resolution
