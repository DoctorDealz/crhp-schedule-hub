# CRHP Schedule Hub

## Project Description

The CRHP Schedule Hub is a web-based schedule and agenda-management tool for retreat weekends, specifically focused on CRHP (Christ Renews His Parish) retreats. It allows event organizers to build, edit, print, and share detailed schedules for each day, specify rooms and team roles, upload/download agenda JSON files, and manage checklists and tasks to keep the event on time.

The hub consists of three tools accessible from the home page (`index.html`):

| Tool | File | Purpose |
|---|---|---|
| 📝 Schedule Editor | `crhp-scheduler.html` | Build and manage the full retreat schedule |
| 👁️ Schedule Viewer | `crhp-viewer.html` | View and track tasks in real time during the retreat |
| 🖨️ Print Service | `print-service.html` | Generate a printable version of the schedule |

---

## Getting Started

Because this is a static web app, no installation or build step is required. Simply open `index.html` in any modern browser to get started.

> **Data storage:** All schedule data is saved to your browser's `localStorage`. No server or account is needed. Use **Export** regularly to back up your data as a JSON file.

---

## How to Use

### 1. Schedule Editor (`crhp-scheduler.html`)

The editor is where you build the retreat schedule. It is divided into four sections in the left-hand panel:

#### Team Roster
- Enter a **Name** and **Role** (e.g., *Lead*, *Support*) and tap **+** to add a person to the roster.
- Tap any roster entry to edit or delete it.
- Roster members can be assigned to tasks in the Task Creator.

#### Room List
- Enter a room name and tap **+** to add it to the list.
- Tap any room entry to edit or delete it.
- Rooms can be assigned to tasks in the Task Creator.

#### Task Creator
Use this panel to add new schedule tasks:
- **Lane** – Choose *Main* (blue, primary tasks) or *Background* (purple, support tasks).
- **Day** – Select which retreat day the task belongs to (the total number of days is configurable in the header).
- **Start / End Time** – Set the task's time window.
- **Task Name** – A short label displayed on the timeline.
- **Assign Rooms / Roster** – Optionally attach rooms and crew members to the task.
- Click **+** to add the task to the schedule.

#### Editing a Task
Tap any task on the timeline to open the edit modal where you can:
- Change the lane, description, status (*Pending* / *Complete*), assigned rooms, and crew.
- **Save Changes** to apply edits.
- **Delete** to remove the task entirely.

#### Timeline Controls (header bar)
- **Day selector** – Swipe or tap arrows to move between retreat days.
- **Lane toggle** (Main / Background) – Filter the timeline to show only one lane.
- **Checklist mode** – Toggle to view all tasks for the day as a flat, checkable list instead of a timeline.
- **Now Line** – A dashed red line automatically moves to show the current time of day.
- **Export (💾)** – Downloads the full schedule as a `.json` file.
- **Import (📂)** – Loads a previously exported `.json` file.
- **Link (↗)** – Opens the Schedule Viewer in a new tab.
- **? (Help)** – Opens the User Guide overlay.

#### Admin Tools (inside the Help menu)
- **Reset to CRHP Master Template** – Restores the default CRHP retreat schedule from the bundled `master_template.json`.
- **Clear All (Fresh Start)** – Wipes all local data so you can start from scratch. Export first!

---

### 2. Schedule Viewer (`crhp-viewer.html`)

The viewer is a **read-friendly** version of the schedule intended for use during the retreat itself. Organizers and team leads can follow along, mark tasks, and monitor progress without accidentally editing the master schedule.

Key differences from the editor:
- Task detail fields are shown as **read-only** by default; only the *Status* field (Pending / Complete) can be updated by team members.
- The **Import (📂)** button loads a schedule JSON that was previously exported from the editor.
- The **Reset** button restores the CRHP master template.
- All other controls (lanes, day navigation, checklist mode, Now Line, Help) work identically to the editor.

**Typical workflow:**
1. Build the schedule in the **Editor** and export it as a JSON file.
2. Open the **Viewer**, import the JSON file.
3. Share the Viewer URL with team members so everyone can follow the live timeline.

---

### 3. Print Service (`print-service.html`)

The print service generates a clean, paginated printout of the schedule.

1. Open the Print Service page.
2. Click **Choose File** (or drag and drop) to load a schedule JSON exported from the editor.
3. The schedule renders on screen grouped by day and lane.
4. Use your browser's **Print** function (`Ctrl+P` / `Cmd+P`) to print or save as PDF.

---

## Data Management

### Exporting
Click **💾 EXPORT** in the editor (or viewer) to download a snapshot of the current schedule as a `.json` file. You will be prompted to name the file before downloading.

### Importing
Click **📂 IMPORT** and select a previously exported `.json` file. You will be asked to confirm before the current data is overwritten.

### Master Template
The repository includes `master_template.json` — a pre-built CRHP retreat schedule that can be loaded at any time via **Reset to CRHP Master Template** in the Help menu.

> ⚠️ **Always export your data before resetting or clearing**, as these actions cannot be undone.

---

## Technical Notes

- **No build step required** – this is a pure HTML/CSS/JavaScript application.
- **Browser compatibility** – Works in any modern browser (Chrome, Firefox, Edge, Safari).
- **localStorage** – Data persists in the browser tab/profile it was created in. Clearing browser data will erase the schedule unless it has been exported.
- **Responsive design** – The UI is optimized for mobile screens and automatically zooms to 170% on desktop displays for easier readability.