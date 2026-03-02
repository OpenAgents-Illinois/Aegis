# Git Commit Standards

## Format

`<type>(<scope>): <description>` (Conventional Commits).

## Types

`feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`.

## Logic

1. Run `git log -n 5` to confirm existing scope naming conventions.
2. Use the imperative mood (e.g., "add connection wizard").
3. **Issue Linking**: If the change resolves an open issue, append `(fixes #ID)` or `(closes #ID)` to the end of the description.
4. **Verification**: Check `.github/prompts/ISSUE_PROMPT.md` to ensure the commit fulfills the requirements defined in the task.

## Example

`feat(ui): connection wizard with test flow (fixes #12)`

## Attribution (co-authors)

When an AI assistant creates the commit, add a co-author line so the commit is attributed to the tool that wrote it. **Use the one that matches the tool you are running in:**

- **If you are in Cursor:** add a line: `Co-authored-by: Cursor Agent <cursoragent@cursor.com>`
- **If you are in Claude Code:** add a line: `Co-authored-by: Claude <noreply@anthropic.com>`

Add this in the commit body (e.g. after a blank line following the subject). The human remains the commit author; the co-author line credits the assistant.
