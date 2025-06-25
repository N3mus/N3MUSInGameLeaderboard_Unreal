# N3MUS Tournament Plugin for Unreal Engine

This plugin allows your Unreal Engine project to integrate with the N3MUS Tournament API.

## Features

- Fetch tournaments using an Auth Token
- Expose tournaments and participants via Blueprint
- Blueprint-friendly design for easy UI integration

## Installation

1. Drop the `Plugins/N3MUSTournament` folder into your Unreal project directory.
2. Regenerate project files (right-click `.uproject` → "Generate Visual Studio project files").
3. Build the project.
4. Enable the plugin in `Edit > Plugins`.

## Usage

1. From Blueprints, create a new object of `TournamentManager`.
2. Call `FetchTournaments(AuthToken)` with your bearer token.
3. Use `GetTournaments()` to access data and bind to your UI.

## Notes

- This is a base version. Customize parsing logic in `TournamentManager.cpp`.
- For mobile webview registration, use `FPlatformProcess::LaunchURL(...)`.

For questions or support, visit: [https://n3mus.com](https://n3mus.com)
