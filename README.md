**Official website:** [https://www.openclawhirehuman.com/](https://www.openclawhirehuman.com/) (ClearPDF)

Collected and curated by the ClearPDF team. **Submissions are welcome.** Open an [issue](https://github.com/c1a1o1/pdf-accessibility-triage/issues/new) or [pull request](https://github.com/c1a1o1/pdf-accessibility-triage/pulls). Include the source, a short description, and any affiliation. We review contributions before adding them.

# PDF Accessibility Triage

Use the [copyable review checklist](CHECKLIST.md) to decide whether to re-export, OCR, or repair a PDF. Searchable, tagged, and navigable are different properties. This is not a conformance audit.

1. **Editable source available?** Fix headings, lists, table headers, document language, form labels, and alternatives for meaningful images before export. Export a tagged PDF when supported. Offer accessible HTML when the fixed layout is not essential.
2. **Classify the pages.** Record text pages, image-only scans, and mixed pages. Copy a passage from each representative layout. If it comes back as gibberish or in the wrong order, check for a better export rather than assuming OCR will fix it.
3. **OCR only where it is needed.** If no better source exists, use an OCR workflow appropriate for the sensitivity of the file. Compare the text with the visible original on every OCR page, especially numbers, names, columns, and tables. OCR alone does not repair tags or reading order. See [W3C PDF7](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF7).
4. **Test two orders separately.** Use a screen reader to listen to the document and check headings, columns, notes, and table headers. Use Tab and Shift+Tab to verify links and form fields have logical focus order and are reachable. See [W3C PDF3](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF3).
5. **Retest the release file.** After a merge or other change, retest each page type and transitions. [ClearPDF Merge PDF](https://www.openclawhirehuman.com/tools/merge-pdf) is our own example for visual page order only; it is not a guarantee of tag preservation or accessibility. Unchecked items are not tested. If a usable PDF cannot be provided promptly, link an accessible alternative beside it.
