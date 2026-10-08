# Trial Master File Control List – BE/BA Studies

A **Trial Master File (TMF)** control list for bioequivalence (BE) and bioavailability (BA) studies. It is a single HTML file: no server, no installation, no build step.

**▶ Use online:** https://mehmetsahin-tr.github.io/trial-master-file-control-list/

The online version runs entirely in your browser. Nothing you enter or attach is uploaded to GitHub or any server; it stays on your own computer. You can also download `trial-master-file-control-list.html` and open it offline.

## Files

- `trial-master-file-control-list.html` – the control list (open in a browser)
- `index.html` – redirects the GitHub Pages address to the control list
- `README.md` – this file
- `LICENSE` – MIT license

## Features

- **Complete / Missing / N/A** status for every document; every document starts as **Please select** until the reviewer chooses
- **Comments with confirmation:** each comment is saved only after the reviewer confirms it, and can be edited later
- **Study details** (title, protocol no., site code, reviewer, review dates) are saved with a button and locked; **Edit details** unlocks them
- **Section check** for sections 1–20: set by the reviewer, never automatically. A checked section is **locked** (no status, comment, attachment or name changes). **Edit** unlocks it after confirmation; the section then needs to be checked again, and its footer and the printout record the check time and how many times it was edited
- **Attach .pdf or .docx files** to any document; PDFs open in a new tab, DOCX files download
- Section 14: renameable **Other List / Form** entries, plus **Add other form** for as many extra forms as needed (each with the same status, comment and attachment options; added forms can be removed)
- Progress bar and counters (total, complete, missing, N/A, not selected, sections checked)
- Filters (all, not selected, missing, complete, N/A) and search by code or name
- **Export / Import** as JSON, including attached files, to move a review between devices or reviewers
- **Print layout:** A4 table with study details, summary, every document with its status, comment and attachment names, section check status, general comments, a sign-off block and page numbers
- Light and dark mode

## Usage

1. Open the online version, or the downloaded file, in a modern browser (Chrome, Edge or Firefox recommended).
2. Fill in the study details and click **Save details**.
3. For each document, change **Please select** to **Complete**, **Missing** or **N/A** (not applicable to the study).
4. Type a comment and click **Save** (or press Enter); confirm it in the dialog. Use **Edit** to change it later.
5. Attach the document if needed.
6. When you have reviewed a section, click the **Check** button at the bottom of the section. To change something later, click **Edit**, make the change and check the section again.
7. Use **Export** to keep a copy, **Print** for a signed paper record.

## Data and privacy

- Statuses and comments are stored in the browser's `localStorage`; attachments are stored in `IndexedDB`. Nothing is sent to a server.
- Clearing browser data deletes the review. Export regularly.
- Large attachments make the export file large, because files are embedded in the JSON.
- **Do not upload documents containing personal subject data** to a public repository or share exports that contain them.

## Customization

The document list lives in the `BASE` array and the sections in the `GROUPS` array inside the HTML file. Edit them to match your site's SOPs. Add `true` as a fourth value to an item to make its name editable.

## Fonts

The interface uses Source Serif 4 and Inter from Google Fonts. Without an internet connection it falls back to system fonts; everything else works offline.

## Disclaimer

This is a **review aid**, not a regulatory text. Always follow your organization's SOPs, current ICH GCP guidance and local regulations.

## License

[MIT](LICENSE) © 2026 Mehmet Şahin. Free to use, modify and share; adapt it to your own templates.
