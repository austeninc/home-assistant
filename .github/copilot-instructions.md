# Copilot Instructions for home-assistant Theme Repository

## Overview
This repository contains Home Assistant theme YAML files and Jinja color reference sheets. The main purpose is to provide visually appealing, platform-inspired themes for Home Assistant, with a focus on iOS and visionOS aesthetics.

## Architecture & Key Files
- `themes/ios-by-austen/ios-by-austen.yaml`: iOS-inspired theme, includes extensive color reference sheets for dark mode and contrast variants.
- `themes/visionos/visionos.yaml` & `Liquid Glass.yaml`: visionOS-inspired themes.
- `jinja-colors.j2`: Jinja template with system color reference sheets for light and contrast modes, useful for generating or referencing color palettes.
- `themes/visionos/readme.md`: Source attribution and minimal documentation.

## Patterns & Conventions
- **Color Reference Sheets**: Each theme YAML starts with a block of color definitions (RGBA and HEX), grouped by mode (light/dark/contrast). These are for reference and not used directly by Home Assistant.
- **Theme Variables**: After the reference sheets, YAML files define Home Assistant theme variables (e.g., `primary-color`, `accent-color`). These follow Home Assistant's theme variable naming conventions.
- **Documentation**: Minimal in-repo documentation. External sources may be referenced in theme readmes.
- **No Build/Test Workflow**: This repo does not use build scripts, tests, or CI/CD. Changes are made directly to YAML/Jinja files.
- **No External Dependencies**: All themes are self-contained. No package management or external integrations.

## How to Contribute
- Add new themes in a subfolder under `themes/` with a descriptive name.
- Start theme files with a color reference sheet for clarity and consistency.
- Follow Home Assistant's theme variable naming conventions.
- Reference external sources in a `readme.md` if adapting from another project.

## Example: Adding a New Theme
1. Create a new folder under `themes/` (e.g., `my-theme/`).
2. Add a YAML file (e.g., `my-theme.yaml`) starting with a color reference sheet.
3. Define Home Assistant theme variables below the reference sheet.
4. Optionally, add a `readme.md` with source attribution or usage notes.

## Key Files to Reference
- `themes/ios-by-austen/ios-by-austen.yaml`
- `themes/visionos/visionos.yaml`
- `jinja-colors.j2`

## Project-Specific Guidance
- Keep color reference sheets up-to-date and consistent across themes.
- Do not add build scripts, tests, or package files.
- Use clear, descriptive folder and file names for new themes.
- Document external sources when adapting themes.

---
For questions about Home Assistant theme variables, see: https://www.home-assistant.io/integrations/frontend/#defining-themes
