# Homebrew Tap

Homebrew casks for [Ghost](https://github.com/ghost-language/ghost) and the
projects built on it.

```sh
brew tap ghost-language/tap
```

## Available

| Cask | Install | Project |
| --- | --- | --- |
| `ghost` | `brew install --cask ghost-language/tap/ghost` | The Ghost programming language |
| `lumen` | `brew install --cask ghost-language/tap/lumen` | A lightweight 2D game engine for Ghost |

Homebrew 6 asks you to trust a non-official tap before it will load anything
from it. Trusting the tap once covers every cask in it, now and later:

```sh
brew trust --tap ghost-language/tap
```

## Casks, not formulae

Both projects ship pre-built binaries rather than building from source, which
is what Homebrew asks a cask to be used for. Casks are macOS-only; on Linux and
Windows, download the archives from the project's own releases page.

The binaries are ad-hoc signed but not notarised, so macOS quarantines them on
download. Each cask clears that attribute on install — without it, the first
run is refused.

## Automation

These files are generated and pushed by each project's release workflow. Edit
them there, not here.
