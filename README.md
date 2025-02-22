# Expo CLI Error: Incompatible Module Import with react-native-web

This repository demonstrates an uncommon error encountered when using Expo's `react-native-web` support. The error arises from attempting to import and utilize modules incompatible with web environments.  Specifically, modules relying on native device features or those designed for Node.js environments fail within a browser context.

## Problem

The core issue is importing modules that assume a native environment (like access to a device camera) into a web-based Expo project.  This leads to runtime errors.

## Solution

The provided solution offers two strategies:

1. **Conditional Imports:** Utilize conditional logic to import different modules based on the environment (web vs. native).
2. **Platform-Specific Modules:** Leverage platform-specific modules where feasible.