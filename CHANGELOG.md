# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.0] - 2026-04-01

### Added

- Drag & drop support for datapoint and element nodes from tree view (#61)
    - Drag DP/element nodes to VS Code editor to insert full DP name at cursor position
    - Drag to external applications (browser, chat, terminal) via system clipboard
    - Full element path is automatically constructed (e.g., `System1:ExampleDP.Value`)
- "Copy DP Name" context menu command for DP and element nodes
    - Right-click on any DP or element to copy its full name to clipboard
    - Confirmation message shown after successful copy

## [0.1.1] - 2026-03-30

### Added

- Multi-platform VSIX build support (linux-x64 and win32-x64)
- Marketplace icon for better visibility in VS Code extensions marketplace

### Fixed

- Security vulnerabilities in npm dependencies
- CI workflow improvements and branch protection rules

## [0.1.0] - 2026-02-15

### Added

- Unified tree view for browsing DPTs, datapoints, and element hierarchies
- Config editor webview for viewing datapoint element configurations
- Display of current values, address configs, alert handling, archive settings
- Value setting through WinCC OA MCP HTTP server integration
- Auto-detection of WinCC OA projects via multiple methods
- SQLite database integration for reading WinCC OA data
- Support for WinCC OA 3.20+ (requires SQLite cache)
