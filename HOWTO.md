# GladargUI: Update Cheat Sheet

Follow these steps whenever you want to push a new version of your strings to CurseForge.

### 1. Update the Code
- Paste new strings into `Core.lua`.
- Update the date in `Core.lua`.
- **Crucial:** Update `## Version: X.X.X` in `GladargUI.toc`.

### 2. Run the Update Batch
Paste this into the VS Code terminal (replace `v1.x.x` with your new version):

```bash
git add .
git commit -m "Update strings"
git tag v1.0.5
git push origin main
git push origin v1.0.5