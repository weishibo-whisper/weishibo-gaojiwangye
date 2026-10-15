---
name: push-gitee
description: Use when committing and pushing this project to Gitee. Trigger on "提交项目", "git commit", "push", "推送", "gitee". Commits changes and pushes to https://gitee.com/weishibo-whisper/advanced-web-pages.
---

# Push project to Gitee

Repository: `https://gitee.com/weishibo-whisper/advanced-web-pages`

## Steps

1. Check state:
   - `git status`
   - `git remote -v`
   - `git log --oneline -5`
2. Stage all changes: `git add -A`
3. Commit with a concise message describing the changes:
   - `git commit -m "<message>"`
4. Ensure the remote exists (add only if missing):
   - `git remote add origin https://gitee.com/weishibo-whisper/advanced-web-pages.git`
5. Push to Gitee:
   - First push: `git push -u origin main`
   - Later pushes: `git push origin main` (or `git push`)

## Notes

- Never commit secrets or credentials.
- If push is rejected because the remote has commits, pull first: `git pull --rebase origin main`, then push again.
- Report the final result (commit hash and push status) concisely.
