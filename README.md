# ValGuide on GitHub 👋

This repository is the shared GitHub home for the `valguide` organization. It holds the organization profile, community guidance, and cross-repository automation that should feel consistent across ValGuide projects.

## What lives here

Use this repository for project-wide material:

* shared GitHub Actions workflows
* composite actions used by more than one repository
* community files such as `CODE_OF_CONDUCT.md`
* the organization profile shown at <https://github.com/valguide> via `profile/README.md`

## Shared automation 🔁

Reusable workflows should live under `.github/workflows/` and be written so repository-specific details are passed in as inputs or secrets. Repositories can then call them like this:

```yaml
uses: valguide/.github/.github/workflows/example.yml@main
```

Keep these workflows boring and stable. If a workflow only makes sense for one repository, it should stay in that repository.

## Community files 📄

GitHub uses community files from this repository when an individual ValGuide repository does not provide its own copy. That makes this a good place for shared contribution, conduct, security, and support guidance.

Repository-local files take precedence. Use local files when a project has different release, support, security, or contribution needs.

## Organization profile

`profile/README.md` is the public landing text for the ValGuide GitHub organization. It should help visitors understand what ValGuide is, where active development happens, and how to find the right project.
