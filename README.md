<div align="center">

# Toolkit

**One desk for every document job.**
Write, highlight, scan, merge, convert, chart and share, all in a single page that runs in your browser.

![Single file](https://img.shields.io/badge/app-single%20HTML%20file-2457f5)
![No upload](https://img.shields.io/badge/files-never%20leave%20your%20device-12805c)
![Themes](https://img.shields.io/badge/theme-light%20%2B%20dark-0f1b2d)
![Status](https://img.shields.io/badge/status-v1%20prototype-ffd84d)

</div>

---

## Why Toolkit

Students, office workers and teams juggle five or six different apps for everyday document work: one for notes, one for PDFs, one for scans, one for converting files, one for charts. Toolkit puts them on one screen, with a section for each goal, so you stop switching tabs and start finishing.

## What's inside

| Tool | What you can do |
|---|---|
| **Write** | Rich text editor with four highlight colours, headings, lists, find and replace, word count and reading time, and autosave. Starts from templates: lecture notes, revision sheet, meeting minutes, memo, report, weekly status, study plan. |
| **Collect highlights** | One click gathers every highlighted line into a revision list you can copy. |
| **Scan to PDF** | Add photos of pages, reorder and rotate them, choose Original, Grayscale or Document cleanup, pick A4, Letter or fit-to-image, and save one PDF. |
| **PDF Studio** | Merge files, extract or delete pages, rotate, add page numbers, stamp a text watermark, and view document info. Page ranges like `1-3, 5, 8-` are supported. |
| **Convert** | Text, Markdown, HTML, CSV and JSON into each other, plus PDF and Word output. Images convert between PNG, JPG and WebP with optional resize. |
| **Charts** | Paste or open a CSV and get a bar, line, pie or ring chart with quick stats (total, average, highest, lowest, change). Save as a PNG. |
| **Share** | Save a note as PDF, Word, text, Markdown and HTML in one go, with a ready-to-send message and copy buttons. |
| **Your desk** | Saved-notes library, recent activity, a weekly goal and a day streak. |

### Built around three goals

- **Students:** lecture notes, highlight collector, handwritten pages to PDF.
- **Office workers:** memos and minutes, merge and split PDFs, numbering and watermarks.
- **Companies and teams:** chart images for slides, weekly status, one report in every format.

### Small things that add up

- Press **Ctrl K** (or **Cmd K**) to jump to any tool.
- Light and dark themes that follow your system or the toggle.
- Works on phone width as well as desktop.
- Notes autosave to your library and reopen where you stopped.
- Files save as normal browser downloads.

## Privacy

Everything runs in the browser. Files you open are read locally and are **not uploaded** anywhere. Notes, activity and settings are kept in the browser's local storage on your device.

## Running it

Toolkit is a single file, `Toolkit.html`. Download it and open it, or use the GitHub Pages site if enabled for this repo. Open it in a modern browser (Chrome, Edge, Firefox, Safari). It loads three libraries from cdnjs, so an internet connection is needed the first time:

| Library | Used for |
|---|---|
| [pdf-lib](https://pdf-lib.js.org/) 1.17.1 | Building, merging and editing PDFs |
| [JSZip](https://stuk.github.io/jszip/) 3.10.1 | Packaging Word (.docx) files |
| [Chart.js](https://www.chartjs.org/) 4.4.1 | Charts |

Fonts: Schibsted Grotesk, IBM Plex Sans and IBM Plex Mono from Google Fonts.

## Known limits (v1)

- **PDF text export is Latin only.** Notes exported to PDF use standard PDF fonts, so Arabic and other scripts do not render correctly yet. Word, text, Markdown and HTML export are fine.
- **No editing inside existing PDFs.** You can reorganise, rotate, number and stamp pages, but not change or highlight the text of an existing PDF.
- **Scans come from uploaded photos.** There is no live camera capture.
- **Local only.** There are no accounts, so notes do not sync across devices.

## Roadmap

- [ ] Arabic and full Unicode PDF export
- [ ] Highlight and annotate inside existing PDFs
- [ ] OCR so scanned pages become searchable text
- [ ] Accounts and cross-device sync
- [ ] Team libraries and shared templates
- [ ] Excel and PowerPoint conversion

## Project structure

```
Toolkit/
├── Toolkit.html   # the whole app: markup, styles and scripts
├── index.html     # redirects to Toolkit.html (for GitHub Pages)
└── README.md
```

## Contributing

Ideas and bug reports are welcome. Open an issue describing what you were doing, what you expected and what happened. For changes, fork the repo, make your edit to `Toolkit.html` and open a pull request.

## Licence

No licence has been chosen yet. Add a `LICENSE` file (MIT is a common choice for a project like this) before inviting outside contributions.
