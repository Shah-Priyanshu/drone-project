# Agent Guidelines for Drone Project

## Project Overview
Custom WiFi-controlled drone development using ESP32 microcontroller and ESP-IDF framework. Currently in planning phase (v1).

## Development Environment
- **Platform**: ESP32 microcontroller
- **Framework**: ESP-IDF (to be installed in WSL)
- **Team**: Pri and Sam

## Build Commands (ESP-IDF - Future)
```bash
idf.py build                 # Build project
idf.py flash                 # Flash to device
idf.py monitor              # Monitor serial output
idf.py clean                # Clean build
```

## Documentation Standards
- **Meeting notes**: Archive in `meeting-logs/` with `YYYY-MM-DD-meeting-notes.md` format
- **Tasks**: Update `TODO.md` with checkboxes and assignee names (- [ ] Task - Name)
- **Versions**: Maintain roadmap in `versioning.md` (v1: WiFi control, v2: Camera+RF, v3: FPV)
- **Components**: Track hardware in `components.md` with categorized checklists
- **Commits**: Use clear messages focusing on "why" not "what"
- **Cross-reference**: Link related files using markdown `[text](file.md)` format

## Code Style (ESP-IDF - Future)
- Follow ESP-IDF naming conventions (lowercase_with_underscores for functions)
- Use `ESP_LOGI/E/W` for logging, include component tags
- Check return values with `ESP_ERROR_CHECK()` for critical operations
- Document complex logic with inline comments
