# welcome-schedule

Welcome Schedule Hub is a browser-based planning tool for **Welcome retreat weekends** (formerly referred to as CRHP).

## Project overview

This repository contains a lightweight static web app used to create, review, and print retreat schedules. The app is designed for coordinators who need to manage agenda timing, roles, rooms, team assignments, and checklist completion throughout a retreat.

## What's included

- **Schedule Editor** (`crhp-scheduler.html`)
  - Build or modify retreat timelines by day
  - Edit task details, assignments, notes, and room information
  - Manage checklist items and completion states
  - Save and load schedules as JSON files
- **Schedule Viewer** (`crhp-viewer.html`)
  - Open schedules in a read-friendly view
  - Follow timeline and checklist progress during the event
- **Print Service** (`print-service.html`)
  - Generate print-ready landscape schedule pages
  - Supports exported schedule data for hard-copy distribution
- **Landing page** (`index.html`)
  - Quick access to editor, viewer, and print tools
- **Master template** (`master_template.json`)
  - Baseline schedule data used as the default retreat template

## Repository name and program naming

- Repository/project name: **welcome-schedule**
- Product context name: **Welcome Schedule Hub**
- Program naming has been updated from “CRHP (Christ Renews His Parish)” to **Welcome**.

## Getting started

Because this is a static HTML/JS project, no build step is required.

1. Clone the repository.
2. Open `/tmp/workspace/DoctorDealz/crhp-schedule-hub/index.html` in a browser.
3. Choose one of the three workflows:
   - Open Schedule Editor
   - View a Schedule
   - Print a Schedule

## Data workflow

1. Start from the bundled `master_template.json` or an existing exported schedule file.
2. Make edits in the editor.
3. Export/share the resulting JSON.
4. Open the same data in the viewer or print service as needed.

## Notes

- Data exchange and session behaviors rely on browser-side storage and file import/export.
- No dedicated package manager scripts, test runner, or build pipeline are currently configured in this repository.
