# Contributing

Thanks for contributing to the chat archiver!

With every change, seek to improve and reduce code.
Leave it better than you found it.

Communicate your intent clearly.
Leave good notes for future devs, including yourself.
Use commit log messages to capture intent.

## Local Development

Build, test, and run the archiver follwing instructions in `Readme.md`.

Serve the `docs/` dir locally with your favorite webserver (e.g. `python -m http`).
You'll want a stylesheet for pretty HTML rendering.
Copy [`docs/assets/` from the Mifos chat archive](https://github.com/mifos/chat-archive/tree/main/docs/assets) into `docs/` or create your own.

The app should be idempotent: Run the archiver again (with the same settings and within the same day window) and confirm no changes are made.

## Submit a patch

Commit only source changes, not generated output.

In the PR description include:

- Reference(s) to JIRA tickets
- What changed (briefly)
- Why it changed (your intent!)
- How you tested locally (automated runs, manual verification, etc.)
- Screenshots for visual changes (before & after)

When updating PRs with new changes, leave commits as-is/un-squashed.
Try to avoid force-pushing.
Use your best judgment here.
In general, only squash/rebase/force push to correct mistakes/noise not helpful for posterity.
If you do force push, make sure collaborators are aware.
It's helpful for posterity / intent forensics to see progress along the way, changes reversed, etc.
Ideally with commit log detail about the "why" for the changes, summaries of our discussions leading to the changes, ideas/plans for future changes, etc.

Note this methodology for source control (keeping a series of PR commits un-squashed) is a different policy than we use for [the apache/fineract repo](https://github.com/apache/fineract).

If/when your patch is merged, confirm the changes are picked up by, e.g. <https://github.com/mifos/chat-archive/>.
