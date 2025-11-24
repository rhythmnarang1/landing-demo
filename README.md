# Landing Demo – Git Merge Conflict Practice

This project is a simple landing page created to intentionally practice Git branching, merging, and resolving merge conflicts. 
## What’s Inside
- `index.html` – basic landing page structure  
- `styles.css` – simple styling  
- `script.js` – small JS interaction  
- `evidence/` – screenshots of the conflict and resolution  
- `REFLECTION.md` – short write-up of what happened and what I learned

## What I Did
1. Created the project locally using Git and pushed it to GitHub.  
2. Made two branches:
   - **feature-header**
   - **feature-hero**  
3. Both branches edited the **same line** in `index.html` (hero section text) to intentionally create a merge conflict.  
4. Merged `feature-header` into `main` first (no conflict).  
5. Then tried merging `feature-hero` → conflict occurred.  
6. Resolved the conflict manually in VS Code by reviewing both versions and combining them.  
7. Committed the resolved file and pushed the final clean version to GitHub.

## Why This Project
The purpose was to clearly understand:
- how merge conflicts happen  
- how Git marks conflicting sections  
- how to resolve them safely using VS Code and Git commands  
- how branches and merges work in distributed version control

## Final Output
The main branch now contains the final merged version of the landing page after resolving the conflict. All screenshots and explanations are included for reference.

