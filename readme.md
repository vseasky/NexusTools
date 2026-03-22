# NexusTools Release Notes

## v0.0.0.1 (2026-03-22)

### New Features
- Unified encoding module (VekEncoding), 26 text encodings supported
- Transmit view (single/multi/periodic) auto-encodes per encoding setting
- Data panel table: delete/send buttons fill cell, header column auto-width
- Table cell text supports selection and copy
- Input caret color follows theme AccentPrimary
- Receive table view unified row height
- Panel tab style unified (contrast, selected/unselected states)
- Floating/docked window rounding and close button fix
- Package script for x64/x86 dual-arch Release build

### Bug Fixes
- Transmit view did not encode text before sending
- Protocol no longer auto-enabled on connect
- Table header `##` prefix rendered as visible text
- VekTable control hover/active background conflicts with row background
