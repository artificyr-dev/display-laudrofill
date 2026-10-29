# LaundroFill: A Liquid Detergent Dispensing Machine

LaundroFill is an IoT liquid dispensing machine that features an LCD touchscreen and sensors that gather data on the laundry and environmental conditions. This information is sent to a central control unit comprised of an Arduino Mega and a Raspberry Pi / host PC. The Arduino handles real-time control of hardware components, while the host manages complex data processing, the user interface, and transaction logging.

---

## Wireframe & Prototype

<a href="https://www.figma.com/proto/I6nTkFidjPWVb5rfQCJt92/LaundroFill-Wireframe?node-id=1-2&node-type=canvas&t=TRBNl7lqfQCOpJpM-0&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1&starting-point-node-id=1%3A2/" target="_blank">
  <img src="Start.png" alt="LaundroFill Wireframe" width="600"/>
</a>

*Click the image above to view the interactive Figma prototype.*

---

## Documentation

- **[ARCHITECTURE.md](ARCHITECTURE.md)**: Hardware pinout, serial protocols, database schema, and detailed sequence diagrams.
- **[REFACTORING_PLAN.md](REFACTORING_PLAN.md)**: Modernization roadmap covering the migration to Vue 3 + Vite, Node.js Express MVC backend, Prisma ORM, Interactive Hardware Simulator, and CI/CD pipelines.

### Current Tech Stack
- **Hardware Controller**: Arduino Mega 2560 (C++ / Wiring)
- **Middleware / Bridge**: Node.js, Express, Socket.IO, `serialport`
- **UI Frontend**: HTML5, CSS3, jQuery, Bootstrap 4
- **Backend & Database**: PHP (Apache/XAMPP), MySQL (`laundrofill_db`)

---

## Project Structure

```text
├── ADMIN/                  # Administrator web dashboard and API scripts
├── USER/                   # Customer kiosk touchscreen interface
├── LAUNDRO_FILL/           # Arduino Mega firmware (.ino)
├── app.js                  # Node.js Serial-to-WebSocket bridge server
├── ARCHITECTURE.md         # Comprehensive architecture and flow diagrams
├── REFACTORING_PLAN.md     # Modernization plan & technical decisions
├── package.json            # Node.js dependencies
└── sales report sample.sql # MySQL sample dataset and schema definition
```
