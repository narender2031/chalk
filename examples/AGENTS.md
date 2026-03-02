# examples

**Parent**: [default](../AGENTS.md)

> Contains illustrative scripts demonstrating advanced terminal styling and animation capabilities. Provides practical examples of dynamic text presentation and ANSI style application.

## Key Concepts

### Semantic Concepts

- **Rainbow Text Colorization with HSL Hue Gradient**: Generates a rainbow-colored string by applying a continuous hue gradient across its characters, preserving non-colorable characters. Calculates the hue progression based on the string's effective length and an initial offset.
- **Terminal Text Animation with Color Cycling**: Animates a given string by applying a rainbow color effect in a continuous loop, updating the terminal output with a short delay between each frame.
- **rainbow.js Concepts**: Aggregates concepts: Rainbow Text Colorization with HSL Hue Gradient, Terminal Text Animation with Color Cycling
- **examples Concepts**: Aggregates concepts: rainbow.js Concepts

### Code Patterns
**Utilities** (2), **Module** (2), **Transformer** (1), **Async/Callback** (1), **Mutator** (1)

## Key Components

### Public API

**Functions:**
- `async function animateString(string) (async)` - Animates a given string by applying a rainbow color effect in a continuous loop, updating the terminal output with a short delay between each frame.
  Calls: rainbow

### Implementation

**Core Functions:**
- `function rainbow(string, offset)` - Generates a rainbow-colored string by applying a continuous hue gradient across its characters, preserving non-colorable characters.

## Folder Overview

### Files

| Name | Summary |
|------|---------|
| `rainbow.js` | Defines functions for generating rainbow-colored text and animating it directly within the terminal. It provides visual utilities for dynamic string presentation. |
| `screenshot.js` | Generates a visual demonstration of various ANSI terminal text styles by iterating through `ansi-styles` keys and applying them with `chalk` to print styled text to the console. It functions as a utility script to showcase the capabilities of the `chalk` library. |

## Dependencies

### Standard Library
- `promises`: Manages asynchronous execution for controlled animation timing within dynamic terminal displays.
- `node:process`: Directs styled output to the standard output stream of the Node.js environment.

### External Packages
- `color-convert`: Transforms color formats to enable dynamic hue gradients for animated text.
- `log-update`: Facilitates flicker-free dynamic terminal output updates for smooth animations.
- `ansi-styles`: Provides a comprehensive set of ANSI style definitions for dynamic text styling demonstrations.

## See Also

- [Parent overview →](../AGENTS.md) - Repository-level concepts and architecture
- [media/ →](../media/AGENTS.md) - Contains static image assets for the application's visual elements. Provides graphical resources such as logos and screenshots for display within the user interface.
- [source/ →](../source/AGENTS.md) - Provides the core implementation for the Chalk library, orchestrating color output, managing ANSI support, and offering string utility functions. It defines the main API and type definitions for text styling, acting as a Facade over complex terminal styling.
- [test/ →](../test/AGENTS.md) - Contains comprehensive test suites for the `chalk` library, validating its core styling capabilities, instance management, and color level control mechanisms. Verifies correct behavior across various scenarios, including hex color application, nested styles, and forced color output.
