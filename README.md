# GitStudio Homebrew tap

The Homebrew cask for [GitStudio Desktop](https://gitstudio.dev), the Git and
GitHub client for macOS, Windows and Linux.

```bash
brew install --cask gitstudiohq/gitstudio/gitstudio
```

That one line taps this repository and installs the app. Add `--force` if you
already have GitStudio.app in /Applications from a direct download.

The cask is generated: `Casks/gitstudio.rb` is written by the release workflow
in [GitStudioHQ/gitstudio](https://github.com/GitStudioHQ/gitstudio) on every
`app-v*` tag, with the checksums read off the uploaded disk images. Please open
issues and pull requests there, not here.

The build is not yet signed with an Apple Developer ID. The cask clears the
quarantine attribute after installing, so the app opens normally; if macOS
still says it is damaged, the cask's caveats (`brew info --cask gitstudio`)
say what to run.
