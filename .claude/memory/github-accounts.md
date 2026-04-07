---
name: GitHub Accounts — Two Profiles
description: Pedro has two GitHub accounts; pedrofer_adobe is enterprise-managed (default gh CLI), maprilpedro is personal. Personal repos must use maprilpedro.
type: user
---

## Pedro has two GitHub accounts with different scopes

- **pedrofer_adobe** — enterprise managed user (Adobe); default active `gh` CLI account; CANNOT create repos (createRepository blocked by EMU policy)
- **maprilpedro** — personal GitHub account; used for personal projects and learning repos

**How to apply:** When creating new GitHub repos for personal projects (like learn-german), always switch to maprilpedro first:
```
gh auth switch --user maprilpedro
# ... create repo, push ...
gh auth switch --user pedrofer_adobe
```
Always switch back to pedrofer_adobe after personal repo operations.
