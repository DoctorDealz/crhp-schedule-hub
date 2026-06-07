# welcome-schedule

Welcome Schedule is a browser-based planning tool for **Welcome retreat weekends**.

## What this tool does

This tool helps your team:

- Build a full weekend timeline
- Assign roles and people
- Track rooms and checklist items
- View and print a clean retreat schedule

No install or build step is required. Open the files in a browser and use the buttons.

## Quick start (non-technical)

1. Open `index.html` in your web browser.
2. Choose one of the three main actions:
   - **Open Schedule Editor** (`crhp-scheduler.html`) to create or update data
   - **View a Schedule** (`crhp-viewer.html`) for read-focused timeline use
   - **Print a Schedule** (`print-service.html`) for print/PDF output
3. If this is your first time, start in **Open Schedule Editor** and load `master_template.json`.

## Most common workflows

### A) Build or update a retreat plan

1. Open **Schedule Editor**.
2. Import the master template or a previously saved JSON file.
3. Update tasks, times, rooms, people, and checklist entries.
4. Export your schedule JSON as a backup and sharing file.

### B) Follow the plan during the retreat

1. Open **View a Schedule**.
2. Import the same JSON you exported from the editor.
3. Use the viewer for a cleaner read-only experience while the retreat is running.

### C) Print or save PDF handouts

1. Open **Print a Schedule** directly, or launch print from editor/viewer.
2. Upload the exported schedule JSON when prompted.
3. Use browser print and select **landscape/horizontal orientation** for best layout.

## Saving, sharing, and backups

- This app stores active edits in browser local storage.
- Export JSON often (especially before clearing cache/resetting data).
- Share schedules by sending the exported JSON file.
- Import that JSON on another device/browser to continue editing or viewing.

## Troubleshooting

### I opened the app and my schedule is missing

- Check if you are using a different browser/profile/device.
- Local storage is browser-specific.
- Import your latest exported JSON backup to restore data.

### Import says the file is invalid

- Confirm the file is valid JSON and came from this scheduler/viewer export.
- Re-export from the source browser if possible and try again.

### Print page is empty or stale

- Upload JSON manually in the print page.
- Refresh the print page after updating data in another tab.
- Re-open print from editor/viewer to send fresh data.

### Buttons that open new pages do not work

- Allow popups/new tabs for your browser session.
- Or open files directly (`crhp-scheduler.html`, `crhp-viewer.html`, `print-service.html`).

## Default role names

The default template includes these role names:

- Retreat Leader
- Formation Leader
- Facilities Leader
- Sacristan
- Invitation/Help Leader
- Kitchen Coordinator
- All Team Members (`ALL`)

You can rename roles in the editor if your parish uses different titles.

## Default witness sessions (ten witness topics)

The default retreat plan includes witness sessions for:

1. Renewal
2. New Life in Christ
3. Spirituality
4. Christian Community
5. Christian Awareness
6. Reconciliation
7. Eucharist
8. Scripture
9. Father's Loving Care
10. Discipleship

## Files included

- **Schedule Editor** (`crhp-scheduler.html`) — create and edit schedules
- **Schedule Viewer** (`crhp-viewer.html`) — open schedules in read mode
- **Print Service** (`print-service.html`) — print-friendly schedule output
- **Landing page** (`index.html`) — opens the three workflows
- **Master template** (`master_template.json`) — default retreat structure and data

## Naming

- Repository/project name: **welcome-schedule**
- Product context name: **Welcome Schedule**
- Existing file names keep the `crhp-` prefix for compatibility with current links/workflows.

## Notes

- Data is handled in the browser through local storage and JSON import/export.
- No package scripts, test runner, or build pipeline are configured in this repository.
