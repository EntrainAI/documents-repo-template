# artifacts

Self-contained deliverables such as HTML previews and reports, one directory
per session: `artifacts/<session id>/<slug>.<ext>`. Only `store_artifact`
writes here, so that each file is recorded and linked from its session's
transcript and Artifacts tab. Don't edit these files by hand. A later session
revises one by passing its path to `store_artifact`.
