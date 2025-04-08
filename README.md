# System Prompts for Book Publishers

![alt text](banner.png)

April 2025

A collection of system prompts designed for fact-checking, proofreading, and text preparation, aimed at book publishers seeking to automate their editorial processes.

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

| Prompt Name | Link | Category | Description | Structured Output |
|-------------|------|----------|-------------|------------------|
| British English Deviation | [![Language](https://img.shields.io/badge/Language-blue)](language/british-english-deviation.md) | Language Standards | Identifies deviations from British English, intended for localizing to other variants of English | [![JSON](https://img.shields.io/badge/JSON-Schema-lightgrey)](structured-output/british-english-structure.json) ✓ |
| Find Inconsistencies | [![Proofreading](https://img.shields.io/badge/Proofreading-green)](proofreaders/find-inconsistencies.md) | Proofreading | Attempts to identify any inconsistencies in the text (highly useful) | - |
| General Proofreader | [![Proofreading](https://img.shields.io/badge/Proofreading-green)](proofreaders/general.md) | Proofreading | For general proofreading of text, quite open-ended configuration | - |
| General Proofreader 2 | [![Proofreading](https://img.shields.io/badge/Proofreading-green)](proofreaders/general2.md) | Proofreading | Alternative version of the general proofreader | - |
| Inconsistency Scanner | [![Proofreading](https://img.shields.io/badge/Proofreading-green)](proofreaders/inconsistency-scanner2.md) | Proofreading | Alternative version of Find Inconsistencies | - |
| Typo Finder | [![Proofreading](https://img.shields.io/badge/Proofreading-green)](proofreaders/typo-finder.md) | Proofreading | Self-explanatory: identifies typographical errors | - |
| Flag Outdated Stats | [![Statistics](https://img.shields.io/badge/Statistics-orange)](statistics/flag-outdated-stats.md) | Statistics Validation | Identifies potentially outdated statistics in the text | - |
| FX Identification | [![Statistics](https://img.shields.io/badge/Statistics-orange)](statistics/fx-identification.md) | Statistics Validation | Identifies currency and exchange rates in the text | [![JSON](https://img.shields.io/badge/JSON-Schema-lightgrey)](structured-output/fx-identification-structure.json) ✓ |
| Outdated FX Rates | [![Statistics](https://img.shields.io/badge/Statistics-orange)](statistics/outdated-fx-rates.md) | Statistics Validation | Identifies potentially outdated exchange rates | [![JSON](https://img.shields.io/badge/JSON-Schema-lightgrey)](structured-output/outdated-fx-rates-structure.json) ✓ |
| Stat Checker | [![Statistics](https://img.shields.io/badge/Statistics-orange)](statistics/stat-checker.md) | Statistics Validation | Verifies statistical claims in the text | [![JSON](https://img.shields.io/badge/JSON-Schema-lightgrey)](structured-output/stat-checker-structure.json) ✓ |
| Stat Isolator | [![Statistics](https://img.shields.io/badge/Statistics-orange)](statistics/stat-isolator.md) | Statistics Validation | Isolates statistical claims for verification | - |
| Broken Link Checker | [![URL](https://img.shields.io/badge/URL-red)](url-validation/broken-link-checker.md) | URL Validation | Identifies broken links and suggests replacements | [![JSON](https://img.shields.io/badge/JSON-Schema-lightgrey)](structured-output/broken-link-checker-structure.json) ✓ |
| Blurb Ideation | [![Content](https://img.shields.io/badge/Content-purple)](blurb-ideation.md) | Content Generation | Generates book blurb ideas | - |
| Tagline Ideation | [![Content](https://img.shields.io/badge/Content-purple)](tagline-ideation.md) | Content Generation | Generates book tagline ideas | - |

## Potential Crews for Multi-Agent Frameworks

These prompts can be assembled into different agent teams in multi-agent frameworks. Here are some suggested crews:

### Basic Proofreading Crew
- Typo Finder
- General Proofreader
- Inconsistency Finder
- FX Identification

### Statistical Validation Crew
- Stat Isolator
- Stat Checker
- Flag Outdated Stats
- Outdated FX Rates

### Comprehensive Editing Crew
- Typo Finder
- General Proofreader
- Inconsistency Finder
- Stat Checker
- Broken Link Checker
- British English Deviation (for localization)

### Marketing Preparation Crew
- Blurb Ideation
- Tagline Ideation
- Broken Link Checker
- General Proofreader

Each crew can work in sequence or in parallel depending on the multi-agent framework implementation, with outputs from one agent potentially feeding into the inputs of another.