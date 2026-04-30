# Contributing to Castloop

Thanks for taking an interest. This guide applies to every repo under [github.com/castloop](https://github.com/castloop).

For brand voice rules (sentence case, terminology, etc.), see [STYLE.md](./STYLE.md). Both apply.

---

## Branching

- `main` is always green, deployable, releasable.
- Work on a branch off `main`, named:
  - `feat/<short-description>` — new capability
  - `fix/<short-description>` — bug fix
  - `chore/<short-description>` — tooling, deps, repo plumbing
  - `docs/<short-description>` — docs-only changes
  - `refactor/<short-description>` — internal restructuring
- Open a pull request when ready. Squash-and-merge for feature branches; merge commits are acceptable for refactors that benefit from preserved history.

---

## Commit messages

Castloop uses Conventional Commits with one twist: **the description is capitalized and written in imperative present tense**.

```
type(scope): Capitalize description

Optional body explaining the why, wrapped at ~72 characters.
Reference issues with "Closes #123" or "Refs #123" if relevant.
```

### Allowed types

| Type | When to use |
|---|---|
| `feat` | New user-visible capability |
| `fix` | Bug fix |
| `docs` | Docs-only change |
| `chore` | Tooling, deps, repo plumbing, no behavior change |
| `refactor` | Internal restructuring without behavior change |
| `test` | Add or modify tests |
| `perf` | Performance improvement |
| `build` | Build-system or external-dep change |
| `ci` | CI config change |
| `style` | Formatting, whitespace, no logic change |

### Scope

A short noun for the area touched. Examples by repo:

- `homepage`: `hero`, `footer`, `meta`, `assets`, `ci`
- `core`: `runtime`, `memory`, `canon`, `routing`, `ffi`, `inference`, `cost`
- `unreal`: `plugin`, `component`, `blueprint`, `ffi`
- `unity`: `runtime`, `editor`, `ffi`, `samples`
- `cli`: `validate`, `build`, `new`, `doctor`
- `canon-format`: `spec`, `schema`, `validators`, `examples`
- `authoring`: `editor`, `canon`, `sandbox`, `bridge`
- `docs`, `.github`, `examples`: usually omit or use `repo`

Drop the scope if the change is repo-wide and a scope would be redundant.

### Examples

```
feat(hero): Add primary CTA button with mailto link
fix(ffi): Free C string returned by last_error_message
docs(brand): Document amber-on-charcoal contrast threshold
chore(repo): Initialize Astro project
refactor(memory): Split SQLite layer from vector index
test(canon): Add golden test for missing-relationship error
```

### Rules

- One concern per commit. Smaller is better.
- Imperative present tense: "Add", "Fix", "Update" — not "Added", "Fixes", "Updates".
- Capitalize the first word after the colon.
- No trailing period in the subject line.
- Keep the subject under 72 characters.

---

## Pull requests

- Keep PRs small and focused. One concern per PR.
- The PR title follows the same convention as a commit subject.
- Describe the **why** in the body. The diff shows the what.
- Link related issues.
- CI must pass before merge.

---

## Pre-merge checklist

Before merging anything to `main` on a public repo:

- [ ] Brand voice rules followed (see [STYLE.md](./STYLE.md))
- [ ] No accidental secrets or credentials
- [ ] No references to internal codenames or rejected names
- [ ] Tests added or updated for code changes
- [ ] Docs match the implementation
- [ ] Performance budgets met where applicable

---

## Filing issues

- **Bugs**: use the bug report template
- **Feature ideas**: use the feature request template
- **Security**: do **not** open a public issue. See [SECURITY.md](./SECURITY.md).

---

## Code of conduct

Participation in any Castloop repo is governed by [CODE_OF_CONDUCT.md](./CODE_OF_CONDUCT.md).
