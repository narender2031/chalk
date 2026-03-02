# supports-color

**Parent**: [vendor](../AGENTS.md)

> 4 files, 6 functions

## Key Components

### Public API

**Functions:**
- `function createSupportsColor(stream?: WriteStream, options?: Options): ColorInfo` - Vendored: createSupportsColor
- `function createSupportsColor(stream, options = {})` `(index.js)` - Vendored: createSupportsColor
  Calls: _supportsColor, translateLevel

### Implementation

**Core Functions:**
- `function hasFlag(flag, argv = globalThis.Deno ? globalThis.Deno.args : process.argv)` - Vendored: hasFlag
- `function envForceColor()` - Vendored: envForceColor
- `function translateLevel(level)` - Vendored: translateLevel
- `function _supportsColor(haveStream, {streamIsTTY, sniffFlags = true} = {})` - Vendored: _supportsColor
  Calls: envForceColor, hasFlag

## Folder Overview

### Files

| Name | Summary |
|------|---------|
| `browser.d.ts` | Vendored: browser.d.ts |
| `browser.js` | Vendored: browser.js |
| `index.d.ts` | Vendored: index.d.ts |
| `index.js` | Vendored: index.js |

## See Also

- [Parent overview →](../AGENTS.md) - Repository-level concepts and architecture
- [ansi-styles/ →](../ansi-styles/AGENTS.md) - Vendored: ansi-styles
