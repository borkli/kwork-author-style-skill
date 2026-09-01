# Releasing

This skill is released at curated milestones rather than for every merged pull request.

## Versioning

Use semantic version tags:

- `MAJOR`: an incompatible change to skill behavior, structure, or installation path;
- `MINOR`: a new supported communication mode or a meaningful compatible expansion;
- `PATCH`: a compatible correction to guidance, examples, or metadata.

## Release process

1. Merge reviewed changes into `main`.
2. Confirm the validation workflow is green on the merge commit.
3. Update `CHANGELOG.md` with the release date and user-visible changes.
4. Create an annotated `vMAJOR.MINOR.PATCH` tag and a GitHub Release from that tag.
5. Generate release notes from merged pull requests, then edit them so they describe the actual change to skill users.

Do not create a release from an unreviewed branch or from a commit with a failing validation check.
