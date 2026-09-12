# android-agent site

The GitHub Pages site for android-agent: https://fox-islam.github.io/android-agent-site/

Plain HTML and one stylesheet, served from `main`. No build step.

- `index.html` is the overview: what it does, what it cannot do, the features, installing.
- `changelog.html` is the release history. Add a new `.release` block at the top for each
  version and point it at that version's APK in
  [android-agent-builds](https://github.com/Fox-Islam/android-agent-builds/releases).

The APKs live in that repo, not this one. The source is private.
