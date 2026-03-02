# default

**Location**: Root directory

> Provides foundational project documentation, configuration, and development utilities for the `chalk` library. Contains essential guidelines for community engagement and contribution, alongside legal terms and performance benchmarking tools.

## Repository Overview
**[readme.md](readme.md)**

Documents the Chalk library, providing an overview of its features, installation instructions, and practical usage examples. It functions as the primary introductory guide for users of the project.

## Code Style

- **Indentation**: tabs
- **Naming**: camelCase
- **Error Handling**: Minimal error handling
- **Common Patterns**: Async/await

## Conventions & Guidelines

- [JavaScript Conventions](JAVASCRIPT_CONVENTIONS.md)
- [TypeScript Conventions](TYPESCRIPT_CONVENTIONS.md)
- [Architecture & Development Guidelines](ARCHITECTURE.md)

## Key Concepts

### Semantic Concepts

- **Chalk Library Performance Benchmarking**: Establishes a benchmark suite for the `chalk` library, comparing the performance of applying one, two, or three terminal styles using both direct method chaining and pre-cached style function references. It measures the execution speed of different `chalk` styling patterns.
- **Direct Terminal Color Application**: Applies a red color style to a predefined string using the `chalk` library, typically within a benchmarking context.
- **Chalk Chained Style Application**: Applies two chained Chalk styles, specifically blue foreground and red background, to a fixed string literal for performance measurement.
- **Fluent ANSI Style Chaining**: Applies a sequence of three distinct ANSI styling attributes—blue foreground, red background, and bold text—to a static string literal. This operation demonstrates the fluent chaining capabilities of the `chalk` library for terminal output.
- **Chalk Pre-composed Style Performance**: Executes a pre-composed Chalk styling function, `chalkBlueBgRed`, on a fixed string to measure the performance of applying two cached ANSI styles.

### Code Patterns
**Handler** (3), **Test Suite** (1), **Types/Definitions** (1), **Configuration** (1), **Entry Point** (1)

## Folder Overview

### Folders

| Name | Summary |
|------|---------|
| [examples/](examples/AGENTS.md) | Contains illustrative scripts demonstrating advanced terminal styling and animation capabilities. Provides practical examples of dynamic text presentation and ANSI style application. |
| [media/](media/AGENTS.md) | Contains static image assets for the application's visual elements. Provides graphical resources such as logos and screenshots for display within the user interface. |
| [source/](source/AGENTS.md) | Provides the core implementation for the Chalk library, orchestrating color output, managing ANSI support, and offering string utility functions. It defines the main API and type definitions for text styling, acting as a Facade over complex terminal styling. |
| [test/](test/AGENTS.md) | Contains comprehensive test suites for the `chalk` library, validating its core styling capabilities, instance management, and color level control mechanisms. Verifies correct behavior across various scenarios, including hex color application, nested styles, and forced color output. |

### Files

| Name | Summary |
|------|---------|
| `benchmark.js` | Implements performance benchmarks for the `chalk` library, evaluating the speed of applying one, two, or three terminal styles through both direct method chaining and pre-cached style function references. Benchmarks measure the execution efficiency of various `chalk` styling patterns. |
| `code-of-conduct.md` | Defines the Contributor Covenant Code of Conduct, outlining pledges, behavioral standards, and maintainer responsibilities for fostering an open and welcoming community environment. Establishes guidelines for acceptable and unacceptable conduct among project participants. |
| `contributing.md` | Outlines guidelines for contributing to the Chalk project. It directs potential contributors to a separate Contributor Code of Conduct document. |
| `license` | Defines the legal terms and conditions for using, modifying, and distributing the associated software. Specifies the permissions granted and limitations of liability under the MIT License. |
| `package.json` | Defines the metadata, dependencies, and scripts for the `chalk` Node.js package, specifying its version, description, and module entry points. Establishes the project's configuration for development, testing, and distribution. |
| `readme.md` | Documents the Chalk library, providing an overview of its features, installation instructions, and practical usage examples. It functions as the primary introductory guide for users of the project. |
## Package Manager

Use **npm**: `npm install`

## Testing

```bash
# Run all tests
npm test

# Run single test file
ava path/to/test

# Lint
xo
```

## Do Not

- **Don't add npm dependencies** - vendored code only
- **Don't use Node-only APIs** - must work in browser
- **No side effects on import** - library must be pure

