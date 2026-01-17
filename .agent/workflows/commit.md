---
description: Analyze changes and create an appropriate commit message in Japanese, then execute the commit.
---

# Git Japanese Commit Workflow

This workflow defines the standard procedure for performing Git commits with Japanese messages.

1. **Check Staging Status**
   - Run `git status` and `git diff --cached` to identify files staged for commit.

2. **Analyze Changes and Generate Message**
   - Thoroughly analyze the staged diff and generate a commit message.
   - **OUTPUT LANGUAGE RULE**: The commit message MUST BE IN JAPANESE.
   - **Format Rules**:
     - 1st line: Summary of changes with a prefix (e.g., `[feat]: 新機能の追加`, `[fix]: バグ修正`).
     - 3rd line and beyond (optional): Briefly describe the "why" and impact of the changes.
   - **Style**: Concise, professional, and clear.

3. **Propose to User**
   - Present the generated Japanese commit message to the user and ask for approval.

4. **Execute Commit**
   - Upon user approval, execute `git commit -m "Generated Message"`.
   - Propose `git push` if appropriate.
