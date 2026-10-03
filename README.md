# PokeFocus Android Prototype v0.2

This version is a native Android prototype for Android 12+.

## What it does
- Requests Android Usage Access and reads actual foreground usage totals with UsageStatsManager.
- Lets you choose installed launchable apps to track.
- YouTube is excluded from the picker by default.
- Adds a first-run starter selection: Bulbasaur, Charmander, or Squirtle.
- Shows real Pokémon official artwork loaded from PokeAPI's public sprite repository.
- Rewards are based on total tracked usage today:
  - >120 min: no reward
  - 61–120 min: Squirtle (common)
  - 21–60 min: Eevee (rare)
  - 1–20 min: Pikachu (very rare)
  - 0 min: Mew (exceptional)
- Includes a launcher/home intent declaration, but this prototype is primarily the tracking/reward app and is not yet a complete launcher replacement.

## Important
The project has not been compiled in this environment because an Android SDK/Gradle installation is unavailable here. It is source code for building an APK in an Android build environment.

The app uses Android's PACKAGE_USAGE_STATS / UsageStatsManager APIs. The user must grant Usage Access in Android Settings. Android documents PACKAGE_USAGE_STATS as the permission for collecting component usage statistics, and UsageStatsManager as the API for querying device usage statistics.

Pokémon artwork is fetched from PokeAPI's sprite repository at runtime rather than bundled into the APK, keeping the app small. Review Pokémon/Nintendo/The Pokémon Company's licensing terms before publishing or commercializing the app.
