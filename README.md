# RCCG Voice of Jesus — Children's Church Check-In

A touch-friendly, offline-capable attendance app for tracking **children** and **staff**
check-in / check-out at children's church. Designed to run on a tablet at the welcome desk.

## Run it

Just open the file — no install, no server, no internet needed.

```
open index.html        # macOS
```

Or double-click `index.html` in any modern browser (Chrome, Safari, Edge).
To "install" it on a tablet, open the page and use **Add to Home Screen**.

## What it does

- **Big tap targets** — tap a person's card to check in, tap again to check out.
- **Children & staff** tracked separately, with live "present now" counts at the top.
- **Pickup security codes** — every child gets a 4-digit code (auto-generated or set
  manually). The code is shown to the guardian at check-in and must be entered on the
  keypad to check the child out, so children are only released to the right person.
- **Allergy / medical notes** surface a ⚠ warning on the card and at check-in.
- **Service date selector** — keep separate records per Sunday/service.
- **Reports tab** — see everyone checked in for the selected service, plus
  **Export CSV** and **Print roster** for records.
- **Roster management** — add, edit, and remove children and staff.

## Data & privacy

- All data is stored **locally in the browser** (`localStorage`) on that device.
  Nothing is sent anywhere.
- Because it's per-device, use the **same tablet/browser** each service, and use the
  CSV export for backups/records.
- To clear sample data: open the Roster tab and delete the example entries, or clear
  the site's storage in browser settings.

## Tech

Single self-contained `index.html` (HTML + CSS + JavaScript, no dependencies).

### Want multi-device sync?
This local-first version is the fastest to deploy. If you later need several tablets
sharing one live roster, it can be extended with a small backend (e.g. Firebase or a
shared database) — ask and it can be added.
