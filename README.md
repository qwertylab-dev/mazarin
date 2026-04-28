# Mazarin

A free Android ebook reader powered by [Project Gutenberg](https://gutenberg.org).

Named after the **Mazarin Bible** — the first major book printed with movable type by Johannes Gutenberg (~1455).

## Features

- Browse and download 70,000+ free ebooks from Project Gutenberg
- Built-in EPUB reader with customizable typography
- Import your own EPUB books
- Material You design with light/dark themes
- Reading progress tracking
- Multi-language support

## Tech Stack

- 100% Kotlin
- Jetpack Compose + Material 3
- Dagger Hilt (DI)
- Room (database)
- OkHttp (networking)
- Coil (image loading)

## Building

```bash
git clone https://github.com/qwertylab/mazarin.git
cd mazarin
echo "sdk.dir=/path/to/Android/Sdk" > local.properties
./gradlew assembleDebug
```

## Credits

Mazarin is a fork of [Myne](https://github.com/Pool-Of-Tears/Myne) by Starry Shivam, licensed under Apache 2.0.

## License

```
Copyright 2024-Present QwertyLab

Licensed under the Apache License, Version 2.0
```
