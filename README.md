# welcome-schedule

Welcome Schedule is a browser-based planning tool for **Welcome retreat weekends**.

## What this tool does

This tool helps your team:

- Build a full weekend timeline
- Assign roles and people
- Track rooms and checklist items
- View and print a clean retreat schedule

No install or build step is required. Open the files in a browser and use the buttons.

## Simple start guide (non-technical)

### Step 1: Open the tool

1. Open `index.html` in your web browser.
2. You will see three main buttons:
   - **Open Schedule Editor**
   - **View a Schedule**
   - **Print a Schedule**

### Step 2: Create or update a schedule

1. Click **Open Schedule Editor**.
2. Load `master_template.json` to start from the default retreat plan.
3. Update task times, notes, rooms, and assigned people.
4. Add or adjust checklist items as needed.
5. Save/export your updated schedule JSON file.

### Step 3: Use the schedule during retreat

1. Click **View a Schedule** and open your saved JSON file.
2. Use the read-only view to follow the retreat timeline.
3. Click **Print a Schedule** to generate print-friendly schedule pages.

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
