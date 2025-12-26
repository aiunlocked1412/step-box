---
description: Update existing workflow steps documentation
---

# Step Box - Update Workflow Documentation

You are a project workflow updater. Refresh the existing STEP-BOX.md file with updated analysis.

## Instructions

1. **Check for Existing Documentation**
   - Look for `STEP-BOX.md` in the project root
   - If not found, inform user to run `/step-box:step` first

2. **Re-analyze the Project**
   - Follow the same analysis process as `/step-box:step`
   - Compare with existing documentation if available
   - Identify new files, removed files, or changed structure

3. **Update the Documentation**
   - Preserve the same format as the original
   - Update the "Last Updated" timestamp
   - Add/remove/modify steps as needed
   - Keep any manual annotations if present (marked with `<!-- KEEP -->`)

4. **Show Changes Summary**
   After updating, provide a diff-like summary:

```
🔄 Step Box Updated!

📄 Updated: STEP-BOX.md
🕐 Updated at: [timestamp]

📊 Changes:
  ✅ Added: [list new steps or files]
  ❌ Removed: [list removed steps or files]
  🔄 Modified: [list changed steps]

Total Steps: [N] (was [M])
```

5. **Handle Edge Cases**
   - If no STEP-BOX.md exists:
     ```
     ⚠️ No existing STEP-BOX.md found!

     Please run /step-box:step first to generate the initial documentation.
     ```

   - If no changes detected:
     ```
     ✅ Step Box is up to date!

     📄 File: STEP-BOX.md
     🕐 Checked at: [timestamp]

     No changes detected since last update.
     (Timestamp updated anyway)
     ```

6. **Update Timestamp Format**
   Always update the timestamp in the format:
   ```
   > Last Updated: YYYY-MM-DD HH:mm:ss
   ```

## Preserve User Customizations

If the user has added custom sections marked with:
```markdown
<!-- CUSTOM START -->
[User's custom content]
<!-- CUSTOM END -->
```

These sections should be preserved during updates.
