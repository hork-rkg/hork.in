# HORK 1.0 — Build 23

Build 23 fixes account and sign-in handling when clearing business content.

- **Clear business content** now removes only the company’s operational records while preserving the HORK company, owner account, users, roles, licences, and sign-in identity.
- The clear-content flow also clears the matching cloud business snapshot so erased records do not silently return during the next sync.
- Remembered sign-in remains available across app updates and ordinary relaunches; the account password is requested again only after the Mac restarts, according to the existing startup security setting.
- Includes the complete Build 22 trade, people, invoice, Goods Return, Leads & Follow-ups, export, layout, responsiveness, and accessibility improvements.

This update does not erase existing business records during installation.
