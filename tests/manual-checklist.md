# Manual test checklist: Favorite Movie page

Open `src/index.html` in a browser (see the README). Mark each item `Pass` or
`Fail` and note the date and browser.

Last run: 2026-10-24, built-in browser pane (Chromium), page served from a throwaway local static server so that `styles.css` loads (the pane shows `file://` pages as a static snapshot without the stylesheet). Items 1 to 5 and 8 were read from the DOM; item 6 from the resource list; item 7 at a 375 px wide viewport (scroll width equals client width).

| # | Check | Expected | Result |
| --- | --- | --- | --- |
| 1 | Exactly one `h1` | Text is "The Best Movies According to Tirsvad" | Pass |
| 2 | Exactly one `h2` | Text is "My top 3 movies of all-time." | Pass |
| 3 | Exactly one `hr` | A horizontal rule sits between the subtitle and the movies | Pass |
| 4 | Three `h3` in order | 13 element, 5th element, Drive | Pass |
| 5 | Each `h3` is directly followed by a `p` | Three paragraphs with the reasons | Pass |
| 6 | No external request | The network log shows only `index.html` and `styles.css` | Pass |
| 7 | Narrow window (375 px wide) | Text wraps and nothing scrolls sideways | Pass |
| 8 | Page title | The tab shows "The Best Movies According to Tirsvad" | Pass |
