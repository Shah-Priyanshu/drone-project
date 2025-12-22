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

## Raw Notes
```
22-12-25:

want to do propellor spped control to change the dir. not individual servos for each propellor to change the drone direction.

material list discussed:
1400kv motor for propellors x4 : https://www.aliexpress.com/item/1005006657243441.html?spm=a2g0o.cart.0.0.441a38daT52zI0&mp=1&pdp_npi=5%40dis%21CAD%21CAD%2015.28%21CAD%2015.28%21%21CAD%2015.28%21%21%21%402101c59117664185397922883e7b72%2112000037941505752%21ct%21CA%216931748317%21%214%210
Simonk30A quadcopter multi-axis drone ESC brushless electronic speed control : https://www.aliexpress.com/item/1005010216203943.html?spm=a2g0o.productlist.main.1.f04cgIBOgIBOjq&algo_pvid=8ff3d056-a891-4d4e-ba51-a6f6d6d54b92&algo_exp_id=8ff3d056-a891-4d4e-ba51-a6f6d6d54b92-0&pdp_ext_f=%7B%22order%22%3A%228%22%2C%22eval%22%3A%221%22%2C%22fromPage%22%3A%22search%22%7D&pdp_npi=6%40dis%21CAD%2121.35%215.52%21%21%21106.40%2127.53%21%402101e2b417664183847831700e3171%2112000051558108571%21sea%21CA%216931748317%21ABX%211%210%21n_tag%3A-29910%3Bd%3Aab1ee60c%3Bm03_new_user%3A-29895%3BpisId%3A5000000187429821&curPageLogUid=tSi0YtsyVSkM&utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005010216203943%7C_p_origin_prod%3A
lipo battery : 220mah 

esp32 module as drone controller


Order 1 of each for inteegration testing and order more after the tests.
```
