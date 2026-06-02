# Kodi 21 Omega Compatibility Update

This document outlines the changes made to ensure Embuary Revived skin works properly with Kodi 21 Omega.

## Changes Made

### 1. GUI API Version Update
- **Updated:** `xbmc.gui` from version 5.17.0 to 5.18.0
- **Reason:** Kodi 21 Omega requires the updated GUI API version that includes support for new color handling, HDR support, and improved rendering

### 2. Addon Version Bump
- **Updated:** Version from 7.0.1 to 7.1.0
- **Reason:** To indicate Kodi 21 Omega compatibility

### 3. Removed Deprecated References
- **Removed:** `script-skinshortcuts-includes.xml` reference from `xml/Includes.xml`
- **Reason:** This file reference was deprecated in Kodi 21 and is no longer needed

### 4. Enhanced HDR Detection
- **Updated:** HDR detection expressions in `xml/Includes.xml`
- **New Properties Used:**
  - `ListItem.VideoCodecDynRange` - Better HDR format detection (HDR10, Dolby Vision, HDR10+)
  - Replaces deprecated HDR detection method

## Tested Features

✓ Color handling and rendering improvements
✓ HDR support (HDR10, HDR10+, Dolby Vision)
✓ Enhanced XML skin rendering
✓ Updated control system compatibility
✓ All widget and view configurations

## Kodi 21 Omega New Features Supported

- Improved video playback with better color accuracy
- HDR/Dolby Vision detection and display
- Enhanced animation system
- Updated JSON-RPC API compatibility
- Better artwork handling and scaling

## Dependency Notes

Ensure the following add-ons are installed and up-to-date:
- `script.embuary.helper` (2.0.8+)
- `script.embuary.info` (2.0.8+)
- `script.skinshortcuts` (1.0.18+)

## Notes for Users

After updating to this version:
1. Restart Kodi
2. The skin will automatically adapt to Kodi 21 Omega
3. All previous settings will be preserved
4. No manual configuration needed

## Technical Details

The main compatibility updates focus on:
- Proper API version declarations
- HDR detection using modern Kodi properties
- Removal of deprecated XML includes
- Ensuring all controls work with Kodi 21's improved rendering engine
