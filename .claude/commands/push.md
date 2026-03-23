---
description: Commit all changes and push to remote
allowed-tools: [Bash(git status:*), Bash(git diff:*), Bash(git log:*), Bash(git add:*), Bash(git commit:*), Bash(git push:*)]
---

# Commit and Push

Commit all current changes and push to the remote repository.

## Instructions

1. Run `git status` to see all changed and untracked files
2. Run `git diff` to review the changes
3. Run `git log --oneline -5` to check recent commit message style
4. If there are no changes, inform the user and stop
5. Stage all changed and new files with `git add -A`
6. Create a concise, meaningful commit message based on the changes:
   - Summarize what was added, changed, or removed
   - Follow the existing commit message style from the repo
   - Keep it short (1-2 sentences)
7. Commit the changes using a HEREDOC format:
   ```
   git commit -m "$(cat <<'EOF'
   commit message here

   Co-Authored-By: Claude Opus 4.6 (1M context) <noreply@anthropic.com>
   EOF
   )"
   ```
8. Push to the remote with `git push`
9. Confirm success to the user with the commit message and branch name

## Rules

- Do NOT force push
- Do NOT amend existing commits
- Do NOT skip hooks (no --no-verify)
- If the push fails, inform the user and suggest next steps
