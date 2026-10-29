# Contributing to GabeTeX

Thank you for taking the time to help! Every bug report, idea, translation fix and pull request is welcome.

**You can write issues and pull requests in English or in Portuguese** (Português do Brasil). Both are equally
welcome; the maintainer reads both. This project follows the [Code of Conduct](CODE_OF_CONDUCT.md). To report a
security problem privately, see [SECURITY.md](SECURITY.md).

## Which repository?

GabeTeX is one project in several repositories. This one is the umbrella; the apps live in the submodules.

| You want to change or report... | Go to | Guide |
|---|---|---|
| The macOS app (Swift, SwiftUI/AppKit) | [GabeTeX-macOS](https://github.com/gabe-rbo/GabeTeX-macOS) | [CONTRIBUTING](https://github.com/gabe-rbo/GabeTeX-macOS/blob/main/CONTRIBUTING.md) |
| The Linux app (Tauri 2, in development) | [GabeTeX-Linux](https://github.com/gabe-rbo/GabeTeX-Linux) | [CONTRIBUTING](https://github.com/gabe-rbo/GabeTeX-Linux/blob/main/CONTRIBUTING.md) |
| The Windows app (Tauri 2, in development) | [GabeTeX-Windows](https://github.com/gabe-rbo/GabeTeX-Windows) | [CONTRIBUTING](https://github.com/gabe-rbo/GabeTeX-Windows/blob/main/CONTRIBUTING.md) |
| The website (`docs/`), the READMEs, community files, templates | this repository | below |
| An idea that spans platforms, or you are not sure | this repository (open an issue) | below |

## Issues

1. Search the existing issues in the relevant repository first.
2. Open the issue in the platform repository when the problem is specific to one app. The issue chooser here links
   to each one.
3. For bugs, include the app version, your OS version and, if you can, a minimal project that reproduces it.
4. Cross-platform ideas: open an issue here and mention the platforms involved. Maintainers may mirror it into the
   platform repositories.

## Pull requests

1. For anything non-trivial, open an issue first so we can agree on the approach.
2. Fork the relevant repository, create a branch, and keep the change focused (one topic per PR).
3. Follow the checklist and conventions in that repository's CONTRIBUTING and PR template.
4. Open the PR against `main` and link the issue (`Closes #123`).

## Working on the umbrella repository

```sh
git clone --recurse-submodules https://github.com/gabe-rbo/GabeTeX.git
cd GabeTeX
```

If you cloned without `--recurse-submodules`, run `git submodule update --init`.

- Website changes go in `docs/`. It is plain HTML, CSS and JavaScript (no build step); open `docs/index.html` in a
  browser. Keep it working in Light and Dark mode, in English and in Portuguese, and keep release/download links
  pointing at the platform repositories.
- Do not commit app code here. Submodule pointers are updated by the maintainer after a change lands in a platform
  repository.
