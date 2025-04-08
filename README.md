# System Prompts for Book Publishers

April 2025

A comprehensive collection of system prompts designed for fact-checking, proofreading, and text preparation, aimed at book publishers seeking to automate their editorial processes.

## Overview

This repository contains specialized system prompts optimized for Gemini 2.5, which can handle entire book manuscripts and offers a long output window. These prompts are designed to assist publishers with various aspects of the editorial workflow, from proofreading and fact-checking to URL validation and statistical verification.

## Key Features

- **Optimized for Gemini 2.5**: All prompts are designed to work with Gemini 2.5's capabilities to process entire book manuscripts
- **Structured Output**: Many prompts include suggested JSON structures for consistent, machine-readable results
- **Specialized Tools**: Categorized prompts for different editorial needs
- **Ready to Use**: Copy and paste these prompts directly into your Gemini interface

## Categories

### Proofreading
- Typo detection and correction
- Inconsistency scanning (character names, dates, etc.)
- General proofreading and copy editing

### Statistics Validation
- Outdated statistics flagging
- Statistical claim verification
- Data isolation and verification
- Currency and exchange rate identification
- Outdated exchange rate detection

### URL Validation
- Broken link detection and replacement suggestions

### Language Standards
- British English deviation detection

### Content Generation
- Blurb and tagline ideation

## Usage

1. Select the appropriate system prompt for your task
2. Copy the prompt text
3. Paste into Gemini 2.5's system prompt field
4. Upload your manuscript or paste the relevant section
5. For prompts with structured output, refer to the corresponding `structure.json` file in the `structured-output` folder

## Directory Structure

| Prompt Name | Link | Relative Link | Badge | Category | JSON Structure |
|-------------|------|---------------|-------|----------|----------------|
| British English Deviation | [Link](language/british-english-deviation.md) | `language/british-english-deviation.md` | ![Language](https://img.shields.io/badge/Language-blue) | Language Standards | [JSON](structured-output/british-english-structure.json) |
| Find Inconsistencies | [Link](proofreaders/find-inconsistencies.md) | `proofreaders/find-inconsistencies.md` | ![Proofreading](https://img.shields.io/badge/Proofreading-green) | Proofreading | - |
| General Proofreader | [Link](proofreaders/general.md) | `proofreaders/general.md` | ![Proofreading](https://img.shields.io/badge/Proofreading-green) | Proofreading | - |
| General Proofreader 2 | [Link](proofreaders/general2.md) | `proofreaders/general2.md` | ![Proofreading](https://img.shields.io/badge/Proofreading-green) | Proofreading | - |
| Inconsistency Scanner | [Link](proofreaders/inconsistency-scanner2.md) | `proofreaders/inconsistency-scanner2.md` | ![Proofreading](https://img.shields.io/badge/Proofreading-green) | Proofreading | - |
| Typo Finder | [Link](proofreaders/typo-finder.md) | `proofreaders/typo-finder.md` | ![Proofreading](https://img.shields.io/badge/Proofreading-green) | Proofreading | - |
| Flag Outdated Stats | [Link](statistics/flag-outdated-stats.md) | `statistics/flag-outdated-stats.md` | ![Statistics](https://img.shields.io/badge/Statistics-orange) | Statistics Validation | - |
| FX Identification | [Link](statistics/fx-identification.md) | `statistics/fx-identification.md` | ![Statistics](https://img.shields.io/badge/Statistics-orange) | Statistics Validation | [JSON](structured-output/fx-identification-structure.json) |
| Outdated FX Rates | [Link](statistics/outdated-fx-rates.md) | `statistics/outdated-fx-rates.md` | ![Statistics](https://img.shields.io/badge/Statistics-orange) | Statistics Validation | [JSON](structured-output/outdated-fx-rates-structure.json) |
| Stat Checker | [Link](statistics/stat-checker.md) | `statistics/stat-checker.md` | ![Statistics](https://img.shields.io/badge/Statistics-orange) | Statistics Validation | [JSON](structured-output/stat-checker-structure.json) |
| Stat Isolator | [Link](statistics/stat-isolator.md) | `statistics/stat-isolator.md` | ![Statistics](https://img.shields.io/badge/Statistics-orange) | Statistics Validation | - |
| Broken Link Checker | [Link](url-validation/broken-link-checker.md) | `url-validation/broken-link-checker.md` | ![URL](https://img.shields.io/badge/URL-red) | URL Validation | [JSON](structured-output/broken-link-checker-structure.json) |
| Blurb Ideation | [Link](blurb-ideation.md) | `blurb-ideation.md` | ![Content](https://img.shields.io/badge/Content-purple) | Content Generation | - |
| Tagline Ideation | [Link](tagline-ideation.md) | `tagline-ideation.md` | ![Content](https://img.shields.io/badge/Content-purple) | Content Generation | - |

## Contributing

Contributions are welcome! If you have developed effective system prompts for book publishing workflows, please submit a pull request.

## License

[Insert your preferred license here]
