# Mazarin

A free Android ebook reader powered by [Project Gutenberg](https://gutenberg.org). Fork of [Myne](https://github.com/Pool-Of-Tears/Myne) by Starry Shivam, licensed under Apache 2.0.

## Build

Requires `local.properties`. Copy from the template:

```bash
cp local.properties.example local.properties
# edit values
./gradlew assembleDebug
```

`GOOGLE_API_KEY` is optional — without it the app builds and runs, but enriched book metadata from the Google Books API is unavailable.

## Architecture

- 100% Kotlin
- Jetpack Compose + Material 3
- Dagger Hilt for DI
- Room for local persistence
- OkHttp for networking
- Coil for image loading

Package root: `dev.qwertylab.mazarin`. Sources under `app/src/main/java/dev/qwertylab/mazarin/`.

## Pre-release blockers

Before any public release of Mazarin, resolve these (search `git grep "TODO"` for the live list):

1. **Backend dependency** — `BookAPI.baseApiUrl` still points at upstream Myne's private proxy (`myne.abyx.in`). Replace with a QwertyLab-controlled backend or with direct Project Gutenberg APIs.
2. **Placeholder URLs in `Constants.kt`** — Telegram, website, sponsors links assume QwertyLab infrastructure that does not exist yet.
3. **Orphaned drawable** `app/src/main/res/drawable/github_pfp.jpg` (was the avatar fallback before the upstream-maintainer photo was removed; safe to delete in a cleanup pass).

## Fork status

Tracking `Pool-Of-Tears/Myne:main`. Local-only modifications relative to upstream:

- Package rename `com.starry.myne` → `dev.qwertylab.mazarin`.
- Cuneiform tablet launcher icon (replaces book-emoji icon).
- Writing-evolution welcome screen (single-page timeline, replaces three-page intro).
- Playfair Display typography (replaces Pacifico).
- Rebranded user-facing strings, themes, README, CONTRIBUTING, ROADMAP, privacy policy.
- Upstream maintainer avatar removed from About screen.

To pull future upstream changes:

```bash
git remote add upstream https://github.com/Pool-Of-Tears/Myne.git  # one-time
git fetch upstream
git rebase upstream/main
# resolve conflicts (rename pattern: com/starry/myne → dev/qwertylab/mazarin)
```
