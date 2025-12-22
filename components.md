# Components

## Component List

### Core Components (v1 - WiFi Control)

#### Flight Controller
- [x] **ESP32 Module**
  - Role: Main drone controller
  - Features: WiFi connectivity for remote control
  - Status: Selected for v1
  - Notes: Will handle motor control via ESCs and WiFi communication

#### Motors
- [x] **1400kV Brushless Motors**
  - Quantity: 4 (one per propeller)
  - Specification: 1400kV rating
  - Supplier: [AliExpress](https://www.aliexpress.com/item/1005006657243441.html)
  - Status: Ready to order for integration testing
  - Price: ~CAD $15.28

#### ESCs (Electronic Speed Controllers)
- [x] **Simonk 30A ESC**
  - Type: Brushless electronic speed control
  - Specification: 30A current rating
  - Application: Quadcopter/multi-axis drone
  - Quantity: 4 (one per motor)
  - Supplier: [AliExpress](https://www.aliexpress.com/item/1005010216203943.html)
  - Status: Ready to order for integration testing
  - Price: ~CAD $5.52

#### Battery
- [x] **LiPo Battery**
  - Capacity: 220mAh
  - Status: Specification selected, voltage/cell count TBD during testing
  - Notes: Size appropriate for initial testing phase

#### Frame
- [ ] Quadcopter frame
  - Status: To be researched
  - Requirements: Must accommodate 4 motors and ESP32 controller

#### Propellers
- [ ] Propellers (x4)
  - Status: To be researched
  - Requirements: Must be compatible with 1400kV motors
  - Notes: Size will depend on frame and motor specifications

### Electronics & Wiring
- [ ] Power distribution board
  - Status: To be researched
  - Requirements: Distribute power from LiPo to ESCs and ESP32

- [ ] Wiring and connectors
  - Status: To be determined based on component requirements

### Optional Components (Future Versions)
- [ ] Camera (v2+)
- [ ] FPV equipment (v3+)
- [ ] Head tracking hardware (future enhancement)

## Design Decisions

### Flight Control Method
**Decision (2025-12-22)**: Use differential propeller speed control for directional changes
- Standard quadcopter approach
- No individual servos per propeller
- Direction control via varying motor speeds
- See [meeting notes](meeting-logs/2025-12-22-meeting-notes.md) for details

## Procurement Plan

### Phase 1: Integration Testing
Order 1 of each component to validate:
- Component compatibility
- Power requirements
- Physical fit and mounting
- ESP32 control capability

### Phase 2: Bulk Order
After successful integration testing, order additional components for full build

## Related Documentation
- [Meeting Notes - 2025-12-22](meeting-logs/2025-12-22-meeting-notes.md) - Component selection discussion
- [TODO.md](TODO.md) - Component ordering tasks
- [versioning.md](versioning.md) - Version roadmap
