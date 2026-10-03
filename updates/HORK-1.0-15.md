# HORK 1.0 (Build 15)

This update improves day-to-day speed, customer management, inventory editing, and HORK AI.

- Smoother Barcoding table scrolling on older Macs, with lighter row rendering and fewer unnecessary redraws.
- Removes the printer-status badge from the Barcoding header while keeping printer controls inside the label workflow.
- Redesigned customer CRM workspace with a customer table, selected-customer insights, sales trend, purchase cadence, recent invoices, follow-up details, and quick actions.
- Cleaner sales-history date filtering and a simpler invoice summary panel.
- HORK AI now uses GPT by default with Claude fallback, formats answers more clearly, and presents compact user prompts with flat assistant responses.
- The dashboard AI panel starts cleanly and provides useful business-question shortcuts.
- Inventory editing can add multiple colour variants safely; each new colour is created as a separate zero-stock record ready for receiving.
- Exact money handling is preserved throughout the new CRM reporting charts.
- Universal Apple Silicon and Intel Mac support.

Your existing business data is preserved during the update.

## One-time repair for Build 14

Build 14 was published with incorrect updater-service permissions. If HORK shows “An error occurred while running the updater,” quit HORK, download the [notarized Build 15 installer](https://hork.in/updates/HORK-1.0-15.dmg), open it, and drag HORK to Applications. Choose **Replace** when macOS asks. This does not remove the business database. Automatic updates work normally again after Build 15 is installed.
