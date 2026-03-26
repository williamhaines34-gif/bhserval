# AGENTS.md

## Cursor Cloud specific instructions

This repository contains a single self-contained static HTML file (`billy-haines-serval (9).html`) — an interactive resume styled as a Serval ITSM incident ticket. There is no build system, no package manager, no backend, and no dependencies to install.

### Running the application

Serve the file with any static HTTP server:

```
python3 -m http.server 8080
```

Then open `http://localhost:8080/billy-haines-serval%20(9).html` in a browser. Note the URL-encoded space (`%20`) in the filename.

### Key interactive features to test

- **Step navigation**: "Next Step" / "Back" buttons and sidebar step links navigate through 6 resolution steps
- **SLA countdown timer**: Live timer in the top-right corner
- **Activity feed**: Right sidebar updates dynamically as steps progress
- **Close Ticket**: Final step has a "Close Ticket" button that transitions to "Resolved" state

### Notes

- Google Fonts are loaded from CDN; the page works without internet but falls back to system fonts.
- There are no lint checks, automated tests, or build steps for this project.
