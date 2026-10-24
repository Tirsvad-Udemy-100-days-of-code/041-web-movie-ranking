**English** · [Dansk](Usage-da) · [Bahasa Malaysia](Usage-ms)

# Usage

## What is on the page

| Element | Text |
| --- | --- |
| `h1` | The Best Movies According to Tirsvad |
| `h2` | My top 3 movies of all-time. |
| `hr` | A horizontal rule |
| `h3` and `p` (three times) | 13 element, 5th element, Drive, each with a short reason |

## Change the movies

Open `src/index.html` in a text editor and edit the `h3` and `p` pairs. Keep each `p` directly after its `h3`:

```html
<h1>The Best Movies According to Tirsvad</h1>
<h2>My top 3 movies of all-time.</h2>
<hr>
<h3>13 element</h3>
<p>This is my favourite anime. I love the beautiful images.</p>
```

Save the file and reload the browser.

## Check the page

Go through `tests/manual-checklist.md`: one `h1`, one `h2`, one `hr`, three `h3` each followed by a `p`, no external request, and no sideways scroll in a narrow window.
