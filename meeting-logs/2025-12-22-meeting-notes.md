# Meeting Notes - December 22, 2025

## Decisions Made

### Flight Control Design
- **Propeller Speed Control**: Decided to use differential propeller speed control to change drone direction (not individual servos for each propeller)
  - This approach is standard for quadcopters and simplifies mechanical design
  - Direction control achieved through varying motor speeds

## Components Discussed

### Motors
- **1400kV Brushless Motors** (x4)
  - Specification: 1400kV rating
  - Quantity: 4 (one per propeller)
  - Source: [AliExpress Link](https://www.aliexpress.com/item/1005006657243441.html)
  - See [components.md](../components.md) for full details

### Electronic Speed Controllers (ESCs)
- **Simonk 30A ESC**
  - Type: Brushless electronic speed control
  - Application: Quadcopter/multi-axis drone
  - Specification: 30A current rating
  - Source: [AliExpress Link](https://www.aliexpress.com/item/1005010216203943.html)
  - See [components.md](../components.md) for full details

### Power System
- **LiPo Battery**
  - Capacity: 220mAh
  - Note: Specific voltage/cell count to be determined during testing

### Flight Controller
- **ESP32 Module**
  - Role: Main drone controller
  - Features: WiFi connectivity for remote control (v1 requirement)

## Action Items
- [ ] Order 1 of each component for integration testing - Pri & Sam
- [ ] Conduct integration tests with initial component set
- [ ] Order additional components after successful testing

## Next Steps
1. Place initial component orders
2. Set up integration testing environment
3. Validate component compatibility and performance
4. Document test results before bulk ordering

## Related Documentation
- [Components List](../components.md) - Updated with specific part details
- [TODO](../TODO.md) - Action items added
- [Versioning](../versioning.md) - v1 WiFi control phase
