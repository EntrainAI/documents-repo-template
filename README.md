# entrain-docs

This organization's documents repository: plans, research notes, decisions and
other writing that outlives a session, and the artifacts sessions store. Every
Entrain session checks it out at `/workspaces/.entrain-docs`, on its default
branch, so agents and people read and write the same files.

## Layout

- `<topic>.md` and `<topic>/…` at the root: documents about the whole
  organization. Name a document for its subject, not for who wrote it or when.
- `projects/<key>/…`: documents about one project, keyed as in Entrain and in
  the organization repository's `projects/<key>/`.
- `artifacts/<session id>/<slug>.<ext>`: self-contained deliverables such as
  HTML previews and reports. Agents write them only with `store_artifact`,
  which records them so the session's transcript and Artifacts tab link to
  them. Nothing else writes here.

Authorship is in git and in the session that wrote a change, so nothing is
organized by person.

## Writing

Search before writing: extend the document on a subject rather than start a
second one. Edit with git on the default branch: commit, `git pull --rebase`,
push. Resolve a rebase conflict against what the other writer meant, rather
than taking one side. No pull request is needed.

Rewrite this README to say where things go as the repository grows; agents read
it before writing.
