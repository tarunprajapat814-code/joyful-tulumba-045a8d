LEDGERPRO — VERSION 2
1. Extract the ZIP.
2. Open index.html in Chrome or Edge.
3. Keep internet connected so the Excel-reading library can load.
4. Upload the provided ledger-style Excel workbook.
5. Review the ledger and date filters. Use Print / Save PDF or Download CSV.

This version targets the uploaded sample layout (one ledger statement in the first worksheet). It detects the transaction header and ledger title, and calculates a running balance from zero unless an opening balance is explicitly present above the table. The sample workbook does not provide an opening balance, so the report starts at zero. It excludes rows after a "Closing Balance" label.

Important: This is a prototype, not accounting software. Verify the balance sign convention and figures before official use. Online deployment is a separate step; the app uses a browser-loaded Excel library.
