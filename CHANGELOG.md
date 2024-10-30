# Changelog

## V1.0.3 (2024-10-30)

### Changed

- chore: update npm packages

## v1.0.2 (2023-10-04)

### Changed

- fix: type in oauth profile interface (special thanks to @jacobszpz)
- chore: bump oauth to v0.10.0
- chore: update npm packages

## v1.0.1 (2023-05-15)

> There is no change to the codebase, just a version bump to publish to the new npm organisation.

### Changed

- chore: update npm organisation from `@techpass` to `@govtechsg`
- chore: update github actions

## v1.0.0 (2023-05-12) - Official Release

### Changed

- fix: use `const` and `let` instead of `var`
- fix: eslintrc is broken
- docs: mulitple touch ups in many areas
- chore: add `nyc` as code coverage tool
- chore: clean up unused pkgs

## v1.0.0-beta5 (2023-04-27)

### Changed

- fix: user object should be defined by application
- fix: token type should be string as they are unparsed

## v1.0.0-beta4 (2023-04-26)

- fix: define Profile interface locally
- docs: clean up jsdoc for verify function

## v1.0.0-beta3 (2023-04-25)

### Changed

- refactor: use `SessionContext` to hold pkce verifier instead of `appState`
- fix: removed unused `meta` argument from `Session.store()`
- fix: improved type definitions for typescript
- fix: "openid" added to scope even if already present. Take in fix from uptream [PR#99](https://github.com/jaredhanson/passport-openidconnect/pull/99).

### Added

- docs: more jsdocs updates
- docs: add constructor parameter description to README

## v1.0.0-beta2 (2023-04-18)

**Note**: Synced to [v0.1.1](https://github.com/jaredhanson/passport-openidconnect/releases/tag/v0.1.1) upstream release.

### Added

- feat: typescript typings

### Changed

- fix: appState should remain undefined if pkce is false

## v1.0.0-beta1 (2023-03-17)

**Note**: Synced to [v0.1.1](https://github.com/jaredhanson/passport-openidconnect/releases/tag/v0.1.1) upstream release.

### Added

- chore: use eslint and prettier
- chore: reorganised github actions

### Changed

- refactor(BREAKING_CHANGE): token claim `oid` property no longer overwrites `profile.id` and returns as `profile.oid`.

### Security

- chore: updated `mocha` deps to resolve security warnings

## v0.3.3 (2022-09-04)

**Note**: Based on upstream [v0.0.2](https://github.com/jaredhanson/passport-openidconnect/releases/tag/v0.0.2) release.

### Added

- feat: replace `profile.id` with `oid` property from id token claim
- feat: provide pkce support
