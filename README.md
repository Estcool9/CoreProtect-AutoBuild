# CoreProtect AutoBuild

Automatically build the latest public development source of [CoreProtect](https://github.com/PlayPro/CoreProtect).

[**Download the latest build**](https://github.com/Estcool9/CoreProtect-AutoBuild/releases/latest)

> This is an unofficial community build. It is not an official CoreProtect release.

## How to install

1. Open the [latest release](https://github.com/Estcool9/CoreProtect-AutoBuild/releases/latest).
2. Download **`CoreProtect-Development.jar`** from the release assets.
3. Put the JAR in your Minecraft server's `plugins` folder.
4. Restart the server and check the console for errors.

Back up your server and database first. Test development builds on a test server before using them on a live server.

## How it works

- Checks the public `master` branch of the CoreProtect source repository every 6 hours.
- Builds a commit when that commit has not already been published by this repository.
- Uses Maven and Java 25 to compile the source.
- Publishes each successful build as a GitHub Release.
- Supports manual runs from the **Actions** tab.

A new release is created only when a new upstream commit is found. The release title includes the short commit hash so you can identify the source used for the build.

## Compatibility

Compatibility depends on the version of Minecraft and server software supported by the upstream source at the time of the build. These builds may contain unfinished changes or bugs; they are not guaranteed to work on every server version.

## Credits

- CoreProtect source code: [PlayPro/CoreProtect](https://github.com/PlayPro/CoreProtect)
- Build automation: [Estcool9/CoreProtect-AutoBuild](https://github.com/Estcool9/CoreProtect-AutoBuild)

CoreProtect remains the work of its original developers. This repository is not affiliated with or endorsed by the CoreProtect developers.
