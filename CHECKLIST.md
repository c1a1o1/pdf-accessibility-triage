# PDF Accessibility Triage Checklist

Record the document version, review date, viewer and screen reader versions, page ranges checked, and whether an editable source or accessible alternative exists. Use **pass**, **issue**, or **not_tested**. Record a page number and an observation for every issue.

- [ ] Classify pages as text, scan, or mixed. Confirm that selected text copies correctly. Check every OCR page against the visible original for omissions and incorrect names, numbers, symbols, and columns.
- [ ] Confirm title, document language, real headings, lists and table headers. Verify text alternatives for meaningful figures and exclude decorative content from reading order.
- [ ] Listen with a screen reader. Check headings, captions, table header announcements and how columns or notes are read.
- [ ] With Tab and Shift+Tab, verify link and form control order and visible focus. Confirm controls have useful names and are reachable without traps.
- [ ] Retest the release file after merging, export or optimization. Cover all modified pages, each page type, and transitions between documents. Assign an owner and next step for any essential unresolved issue.

## Copyable CSV

```csv
page_range,page_type,check,status,observed,owner,next_step
1-2,text,heading_sequence,not_tested,,,
3,scan,ocr_matches_original,not_tested,,,
4,mixed,screen_reader_order,not_tested,,,
4,mixed,keyboard_focus_order,not_tested,,,
2-4,mixed,final_merge_transitions,not_tested,,,
```

Examples: [W3C PDF3: reading and tab order](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF3) and [W3C PDF7: OCR](https://www.w3.org/WAI/WCAG22/Techniques/pdf/PDF7). This checklist is not a conformance statement.
