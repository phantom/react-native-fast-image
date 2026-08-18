# Repository instructions

## Purpose
This repository contains Phantom's `@phantom/react-native-fast-image` package, a performant React Native image component backed by SDWebImage on iOS and Glide on Android.

## Layout
- `src/`: JavaScript and TypeScript package source.
- `ios/`: native iOS implementation.
- `android/`: native Android implementation.
- `ReactNativeFastImageExample/`: React Native example app used for manual development.
- `ReactNativeFastImageExampleServer/`: server used by the example project.
- `docs/`: development and troubleshooting documentation.

## Development and validation
Use Yarn v1 and keep `yarn.lock` in sync with dependency changes.

- Install dependencies: `yarn --frozen-lockfile`
- Build the package: `yarn build`
- Run tests with coverage: `yarn test --coverage`
- Run the configured linter: `yarn lint`

To exercise native changes, follow `docs/development.md` to link the package into `ReactNativeFastImageExample/`, start Metro, and run the iOS or Android app. This project targets the latest React Native version rather than backporting new features to older releases.
