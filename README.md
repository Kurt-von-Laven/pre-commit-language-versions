# pre-commit-language-versions

Minimal Test Repository For Proposed Renovate Feature

Pre-commit allows you to write Git pre-commit hooks in many programming
languages. For a few of those programming languages, namely Python, Node.js,
Ruby, Rust, and Go, you can specify the default version of the language that
pre-commit should use to execute hooks implemented in that language. Hooks may
override that default if desired. While pre-commit supports many additional
programming languages, it currently only uses the version of those languages
that is available on the system and does not install them itself.

See
[the official pre-commit docs](https://pre-commit.com/#overriding-language-version)
for more details.

It would be ideal if Renovate's pre-commit manager could extract the default
language versions from a [`.pre-commit-config.yaml`](.pre-commit-config.yaml)
and offer to bump them.

To use this repository,
[install Poetry](https://python-poetry.org/docs/#installation) and then run
`poetry install --sync` to install [pre-commit](https://pre-commit.com). You can
then run `poetry run pre-commit run --all-files` to run the pre-commit hooks if
desired.
