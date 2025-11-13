<p align="center">Jellify logo</p>

<p align="center">
  <img alt='Jellify / Music App logo' src='assets/transparent-banner.png' width="600" height="300" />
</p>


[![Latest Version](https://img.shields.io/github/package-json/version/varunkumarcs22055/Music-App?label=Latest%20Version&color=indigo)](https://github.com/varunkumarcs22055/Music-App/releases)
[![publish-beta](https://github.com/varunkumarcs22055/Music-App/actions/workflows/publish-beta.yml/badge.svg?branch=main)](https://github.com/varunkumarcs22055/Music-App/actions/workflows/publish-beta.yml) [![Publish Over-the-Air Update](https://github.com/varunkumarcs22055/Music-App/actions/workflows/publish-ota-update.yml/badge.svg)](https://github.com/varunkumarcs22055/Music-App/actions/workflows/publish-ota-update.yml)

<p align="center">Forked and customized by <strong>@varunkumarcs22055</strong>. This repository is published here as <strong>Music App</strong>, and is also distributed / known as <strong>Jellify</strong> (aka <strong>Jefi</strong>).</p>

<p align="center"><em>Note: this repository is now also Jellify.</em></p>

[![Sponsors](https://img.shields.io/github/sponsors/varunkumarcs22055?label=Project%20Sponsors&color=magenta)](https://github.com/sponsors/varunkumarcs22055) [![Patreon](https://img.shields.io/badge/Patreon-F96854?logo=patreon&logoColor=white)](https://patreon.com/varunkumarcs22055)


## Quick Links

[TestFlight](https://testflight.apple.com/join/etVSc7ZQ)

[![Discord Server](https://dcbadge.limes.pink/api/server/https://discord.gg/yf8fBatktn)](https://discord.gg/yf8fBatktn)

## Contents

- [Info](#info)
- [Downloading](#downloading)
- [Screenshots](#screenshots)
- [Features and Roadmap](#features)
- [Built with](#built-with-good-stuff)
- [Support](#support-the-project)
- [Special Thanks](#special-thanks)


## Info

Music App is an open source music player designed to work with the Jellyfin Media Server (https://jellyfin.org/).

Built with React Native, Music App focuses on a clean and responsive UI, offline playback, and performance for large libraries. It requires a connection to a Jellyfin server to access your media (see https://jellyfin.org/docs/ for server setup).

The app showcases artwork from your library, offers playlist management, offline listening, OTA updates, and features aimed at a pleasant listening experience on mobile devices.

### Background

This app was designed with me and my dad in mind. I wanted us to have a sleek, one stop shop for live recordings of bands we like (read: the Grateful Dead). The UI was designed so that we'd find it instantly familiar and useful. CarPlay / Android Auto support was also a must for us, as we both use CarPlay religiously.

### Recommended Additions

These projects are **not** required to use Music App, but are recommended to enrich your Jellyfin music experience!

- [Apple Music Plugin](https://github.com/lyarenei/jellyfin-plugin-itunes)
  - Really good at fetching missing artist artwork for obscure / less popular artists
- [LrcLib Plugin](https://repo.jellyfin.org/files/plugin/manifest.json)
  - Available in the default plugins catalog
  - Really good at fetching song lyrics
- [Jellyfin Rewind](https://github.com/Chaphasilor/jellyfin-rewind)
  - Gives a recap of your year in music listening similar to other music streaming services
  - [A hosted version is provided here](https://jellyfin-rewind.chaphasilor.xyz/)
- [Spotify Playlist Imports](https://github.com/Viperinius/jellyfin-plugin-spotify-import)
  - Imports a user's Spotify playlists into Jellyfin
  - Can run as a scheduled task
- [AudioMuse-AI](https://github.com/NeptuneHub/AudioMuse-AI) and it's [associated plugin](https://github.com/NeptuneHub/audiomuse-ai-plugin)
  - Performs sonic analysis on your music
  - Creates "smart playlists" based on tempo and mood
- [Jellyfin-RPC](https://github.com/Radiicall/jellyfin-rpc)
  - Displays the content you're currently playing on Discord

## Downloading

### Android

Head to [releases](https://github.com/varunkumarcs22055/Music-App/releases) to download the required .APK directly.

Also there is [obtanium](https://github.com/ImranR98/Obtainium) to which you can add this repository (Music App) as a source to use the above releases as a repository.

For Obtanium, click "Add App", put "https://github.com/varunkumarcs22055/Music-App" as the source URL, and on the next screen toggle "prereleases". You'll now be easily able to keep your local copy in sync with new releases.

### iOS

#### The TestFlight Way

Join the [TestFlight](https://testflight.apple.com/join/etVSc7ZQ) and install the latest version from there

#### The Sideloading Way

Head to [releases](https://github.com/varunkumarcs22055/Music-App/releases) to download the required .IPA directly.

Install via [Altstore](https://altstore.io) or your favorite sideloading utility


## Screenshots

Screenshots have been removed from this fork to keep the repository lightweight. You can still view release artifacts (APKs/IPAs) and their screenshots from the Releases page: https://github.com/varunkumarcs22055/Music-App/releases

If you'd like the original screenshots restored into this repository, tell me and I will add them back into an `assets/screenshots/` folder and update these references.


## Features

### Current

- Available via Testflight and Android APK
  - APKs are associated with each [release](https://github.com/varunkumarcs22055/Music-App/releases)
- Light and Dark modes
- Home screen access to previously played tracks, artists, and your playlists
- Quick access to similar artists and items for discovering music in your library
- Music App playback reporting and [Last.FM Plugin](https://github.com/jesseward/jellyfin-plugin-lastfm) support
- Full Library Browsing
- Playlist support, including creating, updating, and reordering
- Offline Playback
- Support for Jellyfin Instant Mixes
- Over-the-Air Updates
  - Powered by [react-native-nitro-ota](https://github.com/riteshshukla04/react-native-nitro-ota). Incremental app updates can be hosted from a separate App Bundles repository; configure that in your deployment setup.
- Shuffling
- Switching Music Libraries
- Google Cast Support

### Roadmap

#### 1.0.0 (We'll Do It Live!) - Dec 5, 2025
- Android Auto/CarPlay
- Quick Connect Support
- Release on App Store and Play Store
- Storage UI Manager
- Album Screen Redesign
- Playlist Screen Redesign
- Allow Self-Signed Certificates

#### 1.1.0 (Socket To Me Baby) - March '26
- Websocket Support (Server online status)
- Home Screen Updates
- Discover Screen Updates
- Artist Screen Redesign

#### 1.2.0 (We Made a Language For Us Two...) - June '26
- Collaborative Playlists
- App Customization Options
- Desktop Support (Experimental)

#### 1.3.0 (Playin' All Day) - September '26
- Autoplay Integration
- Tablet Support

#### 2.0.0  - December '26
- Gapless Playback
- Jellyseerr Integration
- JellyJam
- EQ Controls

#### 3.0.0 - TBD
- Watch Support

\*This is subject to change


## Built with Good Stuff

[![Made with React](https://img.shields.io/badge/React-19-blue?logo=react)](https://reactjs.org) [![React Native](https://img.shields.io/badge/React-Native-079?logo=react)](https://reactnative.dev) [![Made with TypeScript](https://img.shields.io/badge/TypeScript-5-blue?logo=typescript&logoColor=white)](https://typescriptlang.org) [![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier) [![GitHub License](https://img.shields.io/github/license/varunkumarcs22055/Music-App?color=indigo)](https://github.com/varunkumarcs22055/Music-App/blob/main/LICENSE)

## Run locally

These are minimal steps to get the project running for local development. This repository is a React Native app — follow the platform-specific steps below.

Requirements
- Node.js >= 18
- Yarn (recommended) or npm
- For iOS builds: macOS with Xcode and CocoaPods
- For Android builds: Android Studio / SDK

Quick start (PowerShell)

```powershell
# install dependencies (yarn is recommended)
yarn install

# iOS (macOS only) - install CocoaPods
cd ios; bundle install || echo "bundle not installed"; pod install; cd ..

# start Metro bundler
yarn start

# in another terminal: run app on Android or iOS simulator/device
yarn android
# or
yarn ios
```

If you don't have Yarn installed, use npm:

```powershell
npm install
npm run start
npm run android
npm run ios
```

Notes
- The repository uses `patch-package` as a `postinstall` step; keep that in mind during installs.
- If you encounter native build issues, make sure your Xcode/Android SDK and related tooling are up to date.
- This README contains a short fork attribution and some badge links updated to point at this repository.

### Frontend

[Tamagui](https://tamagui.dev/)\
[Figtree](https://github.com/erikdkennedy/figtree)\
[React Navigation](https://reactnavigation.org/)\
[React Native Blurhash](https://github.com/mrousavy/react-native-blurhash)\
[React Native CarPlay](https://github.com/birkir/react-native-carplay)\
[React Native Draggable Flatlist](https://github.com/computerjazz/react-native-draggable-flatlist)\
[React Native Nitro Image](https://github.com/mrousavy/react-native-nitro-image)\
[React Native Reanimated](https://docs.swmansion.com/react-native-reanimated/)\
[React Native Toast Message](https://github.com/calintamas/react-native-toast-message)\
[React Native Vector Icons](https://github.com/oblador/react-native-vector-icons)

- Specifically using [Material Community Icons](https://oblador.github.io/react-native-vector-icons/#MaterialCommunityIcons)

### Backend

[Jellyfin SDK](https://typescript-sdk.jellyfin.org/)\
[Tanstack Query](https://tanstack.com/query/latest/docs/framework/react/react-native)\
[React Native DNS Lookup](https://github.com/tableau/react-native-dns-lookup)\
[React Native File Access](https://github.com/alpha0010/react-native-file-access)\
[React Native Google Cast](https://github.com/react-native-google-cast/react-native-google-cast)\
[React Native MMKV](https://github.com/mrousavy/react-native-mmkv)\
[React Native Nitro OTA](https://github.com/riteshshukla04/react-native-nitro-ota)\
[React Native Track Player](https://github.com/doublesymmetry/react-native-track-player)\
[React Native URL Polyfill](https://github.com/charpeni/react-native-url-polyfill)\
[Zustand](https://github.com/pmndrs/zustand)

### Opt-In Monitoring

All logging and metrics gathering is _opt-in_ __by default__. This is merely here to help us make Music App better. 

All logs and metrics are completely anonymized. No data can be traced back to you.

[GlitchTip](https://glitchtip.com/)

- [See logging statements](https://github.com/search?q=repo%3Avarunkumarcs22055%2FMusic-App+console.&type=code&p=1)

[TelemetryDeck](https://telemetrydeck.com)

### Love from Wisconsin 🧀

This is a passion project of [mine](https://github.com/varunkumarcs22055). I hope you enjoy using it! Feature requests and bug reports are welcome :)

## Support the Project

You can support Music App development via [Patreon](https://patreon.com/varunkumarcs22055) or [GitHub Sponsors](https://github.com/sponsors/varunkumarcs22055) starting at $1.

Paid supporters will be recognized by having their name displayed within the Settings.

## Special Thanks

- The [Jellyfin Team](https://jellyfin.org/) for making this possible with their software, SDKs, and unequivocal helpfulness.
  - Extra thanks to [Niels](https://github.com/nielsvanvelzen) and [Bill](https://github.com/thornbill)
    - They taught me the ways of the AudioAPI and how to do audio transcoding with Jellyfin
- [James](https://github.com/jmshrv), [Chaphasilor](https://github.com/Chaphasilor) and all other contributors of [Finamp](https://github.com/jmshrv/finamp) - another music app for Jellyfin
  - James’ [API Blog Post](https://jmshrv.com/posts/jellyfin-api/) proved to be exceptionally valuable during development
  - Chaphasilor taught me everything they know about audio normalization and LUFS, and their math was referenced in Music App's audio normalization algorithm
- Marc and the rest of the [Margelo Community](https://discord.com/invite/6CSHz2qAvA) for their amazing modules and support
- [Nicolas Charpentier](https://github.com/charpeni) for his [React Native URL Polyfill](https://github.com/charpeni/react-native-url-polyfill) module and for his assistance with getting Jest working
- The team behind [Podverse](https://github.com/podverse/podverse-rn) for their incredible open source project, of which was used as a reference extensively during development
- My fellow [contributors](https://github.com/varunkumarcs22055/Music-App/graphs/contributors) who have poured so much heart and a lot of sweat into making Music App a great experience
  - Extra thanks to [John](https://github.com/johngrantdev), [Vali-98](https://github.com/Vali-98), and [Erik](https://github.com/felinusfish) for shaping and designing the user experience
  - Shout out to [skalthoff](https://github.com/skalthoff) for championing many features:
    - Gapless Playback
    - Library Selection
    - Quality Selection
  - Many thanks to PDB3D for the logo design!
  - Huge thank you to [Ritesh](https://github.com/riteshshukla04) for literally so many things:
    - Over-the-Air Updates
    - Cast Support
- The friends we made along the way that have been critical in fostering an amazing community around Music App
  - [Thalia](https://github.com/thaliadavar)
  - [BotBlake](https://github.com/BotBlake)
  - [Neptune1987](https://github.com/NeptuneHub)
- My long time friends that have heard me talk about Music App for literally **eons**. Thank you for testing Music App during its infancy and for supporting me all the way back at the beginning of this project
  - Tony (iOS, Android)
  - Trevor (Android)
  - [Laine](https://github.com/lainie-ftw) (Android)
  - [Jordan](https://github.com/jordanbleu) (iOS)
- My best(est) friend [Alyssa](https://www.instagram.com/uhh.lyssarae?igsh=MTRmczExempnbjBwZw==), for your design knowledge and for making various artwork for Music App.
  - You’ve been instrumental in shaping its user experience, my rock during development, and an overall inspiration in my life


## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=varunkumarcs22055/Music-App&type=Date)](https://www.star-history.com/#varunkumarcs22055/Music-App&Date)
