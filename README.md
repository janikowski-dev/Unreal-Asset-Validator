# Unreal Asset Validator

Unreal Engine editor plugin that exports asset metadata and integrates Unreal with an external, engine-agnostic asset validation pipeline.

This plugin handles **editor integration and data export only**.  
All validation logic runs **outside Unreal Engine**.

## Overview

`Unreal Editor → JSON → Asset Validator (Core) → Results` 

-   Unreal Engine: asset selection and metadata extraction
-   External validator: rule evaluation and reporting
    
Core validation logic lives here:  
👉 https://github.com/janikowski-dev/Asset-Validator

## Design principles

-   Clear separation between data export and validation
-   No engine-specific validation logic
-   Reusable across projects and pipelines
-   CI-friendly by design
