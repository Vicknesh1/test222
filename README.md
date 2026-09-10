# FoundryFlow — Foundry Industry Form Prototype

A no-build, GitHub-friendly prototype for a foundry production data-entry form.

## What is included

- Login screen with Admin and User roles
- 81-field foundry heat-production form
- Dropdowns with example master-data options such as Grade: 5A / CF8
- Sectioned layout so the operator can understand the workflow
- Completion progress indicator
- Save/reset behavior using browser localStorage
- Admin-only Field Configuration screen
- Admin can:
  - change a field type
  - rename/edit fields
  - edit dropdown options
  - add a field
  - delete a field
  - restore the original 81-field setup
- Calculation fields are shown as read-only placeholders for the prototype

## Demo login

Admin:
- Email: `admin@foundry.com`
- Password: `admin123`

User:
- Email: `user@foundry.com`
- Password: `user123`

## Run locally

Just open `index.html` in a browser.

## Run on GitHub

1. Create a new GitHub repository, for example `foundry-form-prototype`.
2. Upload `index.html` and this `README.md`.
3. Go to **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**.
5. Select your main branch and `/root` folder.
6. Save. GitHub Pages will publish the prototype.

## Important prototype limitation

This version is frontend-only. The login accounts, form data and field configuration are stored in the browser.

For a real factory deployment, replace this with:
- real authentication
- PostgreSQL / Supabase / PocketBase or another database
- server-side role/permission checks
- audit log
- user/company/site/furnace master tables
- formulas/calculation engine
- validation
- export/reporting
- API integration with PLC/SCADA/MES where required
