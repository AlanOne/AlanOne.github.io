# alanone.github.io

Everything on https://alanone.github.io, from this one repo. `.github/workflows/deploy.yml`
builds and publishes it on every push to `main`.

| URL | From |
|---|---|
| [/undefined-behavior/](https://alanone.github.io/undefined-behavior/) | `undefined-behavior/`, a Hugo blog (PaperMod theme, a submodule). Moved here from AlanOne/undefined-behavior with its history. |
| [/takefive/](https://alanone.github.io/takefive/) | `takefive/`, the Take 5 cheat sheet. Made in the takefive repo and published here by its `scripts/publish-cheat-sheet.sh`; don't edit it here. |

Any other top-level folder is served as it is: add `foo/index.html` for `/foo/`. Missing pages show
the blog's 404 page.

To write a post: add it under `undefined-behavior/content/posts/` and push. To preview locally,
`hugo server --source undefined-behavior` (Hugo extended 0.165.0, as the workflow uses), after
`git submodule update --init` for the theme.
