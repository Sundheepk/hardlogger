# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2026-01-11

### Changed
- **BREAKING**: Migrated from scoped package `@rdrudra99/hardlog` to unscoped `hardlogger`
- Package name changed for better discoverability and professional branding
- Bumped to v1.0.0 to signal production-ready status
- Enhanced npm keywords for better search visibility

### Migration
To upgrade from `@rdrudra99/hardlog`, simply:
```bash
npm uninstall @rdrudra99/hardlog && npm install hardlogger
```
Then update your imports from `'@rdrudra99/hardlog'` to `'hardlogger'`. The API is 100% identical.

### Note
The old scoped package `@rdrudra99/hardlog` will remain available but deprecated. All future updates will be published to `hardlogger`.

---

## [0.1.0] - 2026-01-09

### Added
- Initial release of hardlog
- Auto-detection for Node.js and Browser environments
- ANSI color support for terminal output
- CSS-styled console output for browsers
- Production-safe logging (disabled by default in production)
- Configuration API with `log.config()`
- TypeScript support with full type definitions
- Zero dependencies (only dev dependencies)
- Four log levels: success, error, warn, info
- Optional timestamp support

### Features
- Works in Node.js 14+
- Works in all modern browsers
- Compatible with Next.js (App Router + Pages Router)
- Compatible with Express.js
- Compatible with Bun and Deno
- SSR-safe and edge runtime compatible
- Never throws errors - fails silently
