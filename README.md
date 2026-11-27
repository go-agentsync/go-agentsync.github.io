# go-agentsync.github.io

The landing page for [go-agentsync](https://github.com/go-agentsync), built with
Hugo on the shared [landingkit](https://github.com/go-fleettools/landingkit)
module and deployed by GitHub Actions to <https://go-agentsync.github.io/>.

The brand colours in `hugo.toml` are generated from `static/img/logo.svg`
(`landingkit brand static/img/logo.svg`), never chosen by hand. Cards stay short:
one line, one number, a link; the detail is in each repository's README.

Adding a repository means a `[[params.modules]]` block **and** its name in the
list in `.github/workflows/ci.yml`; a new agentscope release means a
`[[params.releases]]` block. Pages must build from the workflow, not from a branch.

```sh
hugo server
```

BSD-3-Clause.
