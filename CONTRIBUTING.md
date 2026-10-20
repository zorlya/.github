# Contributing to Zorlya

Thank you for helping. This is the default guide for every repository in the Zorlya organization that has no `CONTRIBUTING.md` of its own. Most of our repositories are private and open to the team and invited collaborators. A repository's own `README.md`, `AGENTS.md` and `docs/` always win over this page.

## Before you start

- Read the repository's `README.md` and its docs. The monorepo keeps its docs in `docs/`, starting at `docs/README.md`.
- Look for an existing issue, decision or plan before you build something new.
- One task per issue and per pull request.
- Security problems do not go in issues. Follow [SECURITY.md](SECURITY.md).

## Branches and commits

- Work on a branch, never on `main` or `trunk` directly. Name it `<type>/<slug>`: `feat/`, `fix/`, `docs/`, `chore/` or `refactor/`.
- Write commits as `type(scope): summary`, in the imperative, one scope per commit. Example: `fix(web): link the YouTube channel by its handle`.
- Stage files by name, not with `git add -A`. Keep unrelated changes in their own commits.
- Do not force-push. Bring a branch up to date with `git merge`, not a rebase.
- Do not add `Co-Authored-By` lines, session links or other tool attribution to commits or pull request descriptions.

## Pull requests

Give the description these four sections:

1. **What changed.**
2. **How it was checked:** the commands you ran and what they printed.
3. **Not checked:** say what you did not verify. A pull request that hides this gets sent back.
4. **Rollout and migration notes:** a migration, a new variable, secret or setting, and the order to deploy in. Write "None" when there is nothing.

Put `Closes #N` on its own line for each issue the pull request finishes. Run the repository's checks before you open it; the CI runs the same commands.

Changes to sign in, sessions, tokens, permissions or customer email need a security review before they merge. Name that in the description and say what to check.

Merge with a merge commit. Do not squash.

## Secrets and data

- Never commit `.env`, `.dev.vars`, tokens, keys, passwords or exports that hold user data. Commit `.example` files with placeholders only.
- Never paste a secret into an issue, a pull request, a commit message or a chat.
- A production deploy, a DNS change, a remote database write or a secret change needs the owner's say-so for that action.

## Writing

Anything a user reads, in the product, in docs and in the pull request text, follows the same rules: plain and specific, active voice, no emoji, no exclamation marks, and no number or company fact that the data does not back. Put the brand name in the brand typeface where it is shown on a page.

## Questions

Write to [support@zorlya.com](mailto:support@zorlya.com).
