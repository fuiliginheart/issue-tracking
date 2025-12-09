# Changelog

All notable changes to the Delta Green HUD module will be documented in this file.

## [1.1.0] - 2025-12-09

### Added

#### Bond Projection:
- Bond projection now reduces agent's Willpower by the projected amount
- WP reduction is displayed in the chat message alongside bond score reduction

#### Breaking Point
- BP (Breaking Point) now displays as a unified stat alongside HP, WP, and SAN on both full and compact bars
- Breaking Point indicator integrated into the Sanity bar in the Psych panel, positioned proportionally based on BP value
- Reset Breaking Point button appears on stat bar when BP is reached.
- Reaching BP whispers messages to Agent and Handler

#### Roll Modifiers
- Shift-click on any stat or skill button to open modifier dialog
- Allows fine-tuned +/- modifiers before rolling
- Quick preset modifier buttons for ±20 and ±40 adjustments
- Works for attributes, sanity checks, and skill rolls in both compact panel and full skills panel

#### Dice So Nice Integration
- All rolls (stats, skills, sanity checks, gear) now fully integrate with Dice So Nice
- Rolls display animated dice animations before showing results
- Delta Green system's native roll pipeline is used for all roll types

#### Damage Roll Buttons
- Success and critical success skill/weapon rolls now display contextual damage roll buttons in chat cards
- Successes show "Roll Damage" button with weapon damage
- Buttons span full width of chat card for easy access

### Changed

#### General 
- "Also restore this amount to Agent's SAN?" checkbox in bond projection dialog is now unchecked by default
- Text color in bond projection dialog changed to black (#000) for better readability
- HP, WP, SAN, and BP display now have fixed, equal widths to prevent layout shift when values change from single to double digits
- Increased spacing between stat boxes from 6px to 12px for better visual separation on both full and compact views
- HUD tabs bar width changed from fixed to auto-expanding to accommodate dynamic stat panel width
- Compact rollables panel now auto-expands to match stats bar width instead of fixed width
- BP stat label now uses distinct orange color (#ff8800) for visual consistency

### Fixed
- Willpower reduction is now properly applied when projecting trauma onto bonds
- HUD now correctly re-renders after bond projection to display updated WP
- Unified stat display template for both full and compact views with consistent spacing
