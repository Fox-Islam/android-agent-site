# Android Agent site

The GitHub Pages site for Android Agent: https://fox-islam.github.io/android-agent-site/

View the source code for the app at [Fox-Islam/android-agent](https://github.com/Fox-Islam/android-agent).

Plain HTML and one stylesheet, served from `main`. No build step.

- `index.html` is the overview: what it does, what it cannot do, the features, installing.
- `changelog.html` is the release history. Add a new `.release` block at the top for each
  version and point it at that version's APK in
  [android-agent](https://github.com/Fox-Islam/android-agent/releases).

Two things go stale together, so change them together: the version beside the download
button on `index.html`, and the newest block in `changelog.html`. A changelog entry can only
link to a version that was actually released, which is why the history
starts at 1.1.0 rather than at the first tag.

Pages serves `style.css` with `cache-control: max-age=600`, so for ten minutes after a change
your own browser keeps the old one. A layout that looks broken right after a push is usually
that: hard-reload before believing it.

`media/` holds the screen recordings and screenshots used on the overview. The two videos are
captures from a real phone, nothing cut, though the middle of the Duolingo one is sped up; the
stills come from an emulator. If you re-cut a video, check the caption still describes it. Keep them small, because
GitHub Pages serves them on every visit and the page already carries several megabytes.

The APKs live in that repo, not this one. The source is private.
