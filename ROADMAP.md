# Roadmap

## Phase 1 — Identity (rebrand)

- [x] Define app name → **Mazarin**
- [x] Change package ID → `dev.qwertylab.mazarin`
- [ ] New icon and logo
- [ ] Update splash screen with new branding
- [x] Update About screen (links, credits, description)
- [x] Replace/remove hardcoded Google Books API key
- [x] Change `applicationId`, `versionName`, `versionCode`

## Phase 2 — Code cleanup

- [ ] Migrate everything from Material 2 to Material 3 (drop `compose-material` dependency)
- [x] Clean up deprecation warnings in `gradle.properties`
- [x] Verify `.gitignore` (local.properties, keys, builds)
- [ ] Remove dead or commented-out code
- [ ] Review and clean hardcoded strings (prepare for i18n)

## Phase 3 — Reader improvements

- [ ] Reading themes (light, sepia, dark, AMOLED black)
- [ ] Bookmarks system with Room persistence
- [ ] In-book text search
- [ ] Improved progress slider (jump to position within chapter)
- [ ] Brightness gesture (swipe on left edge)
- [ ] Configurable screen orientation (auto, portrait, landscape)

## Phase 4 — New features

- [ ] Annotations and highlights (highlight + save notes in Room)
- [ ] TTS (text-to-speech) with playback controls
- [ ] Built-in dictionary (tap a word → definition)
- [ ] PDF support
- [ ] Reading stats (time read, pages per day, streaks)
- [ ] Import from more sources (Open Library, Standard Ebooks, Internet Archive)

## Phase 5 — Play Store

- [ ] Create Google Play developer account ($25)
- [x] Draft privacy policy
- [ ] Complete content rating questionnaire
- [ ] Prepare screenshots and store listing (title, description, graphics)
- [ ] First Play Store release
- [ ] Set up CI/CD for automated builds (GitHub Actions)
