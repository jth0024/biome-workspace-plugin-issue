# Biome Workspace Plugin Issue

## Overview

This repo demonstrates that Biome plugins do not work when they are configured in nested `biome.json` files. They only work when they are defined in the root `biome.json` file.

## Steps to Reproduce

To reproduce the issue, perform the following steps:

1. Checkout this repo
2. Run `pnpm install`
3. Run `pnpm exec biome lint -- **/rule-violation.ts`

## Expected Result

Biome reports a linting error from the `noObjectAssign` plugin

## Actual Result

Biome reports no linting errors for the file
