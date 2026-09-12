# Android Agent site

The GitHub Pages site for Android Agent: https://fox-islam.github.io/android-agent-site/

Plain HTML and one stylesheet, served from `main`. No build step.

- `index.html` is the overview: what it does, what it cannot do, the features, installing.
- `changelog.html` is the release history. Add a new `.release` block at the top for each
  version and point it at that version's APK in
  [android-agent-builds](https://github.com/Fox-Islam/android-agent-builds/releases).

Two things go stale together, so change them together: the version beside the download
button on `index.html`, and the newest block in `changelog.html`. A changelog entry can only
link to a version that was actually published to the builds repo, which is why the history
starts at 1.1.0 rather than at the first tag.

The APKs live in that repo, not this one. The source is private.
