# stp

**Simple Teleprompter** — or *s'il te plaît*, if you prefer.

A minimal, standalone teleprompter that runs entirely in your browser — no server, no install, no internet required. Open `stp.html` and go.

---

## Getting started

Download or clone the repo, then open `stp.html` directly in any modern browser (Chrome, Firefox, Safari, Edge).

1. Paste your script into the text area
2. Adjust settings in the top bar to your liking
3. Press **▶ Start**

---

## Controls

### Top bar

The bar has two states: **expanded** (edit mode) and **collapsed** (scrolling mode).

The action buttons are always visible on the left, in the same position regardless of bar state. Click **▾ / ▴** on the far right to toggle settings visibility.

| Button | Action |
|--------|--------|
| ▶ Start / ⏸ Pause / ▶ Resume | Start, pause, or resume scrolling |
| ⏫ Top | Jump to the beginning and pause |
| 📋 TOC | Toggle the Table of Contents panel |
| ↔ | Flip text horizontally (for teleprompter glass) |
| ↕ | Flip text vertically |
| − / + (speed) | Decrease or increase scroll speed |

### Settings (expanded bar)

| Setting | Range | Default |
|---------|-------|---------|
| Font size | 16 – 96 px | 36 px |
| Speed | 1 – 20 | 5 |
| Width | 30 – 100% of viewport | 70% |
| Line gap | 1.2 – 2.5 | 1.6 |
| Align | Left / Center / Right | Center |
| Theme | White on black / Black on white | White on black |

---

## Keyboard shortcuts

These work while text is scrolling (not while editing).

| Key | Action |
|-----|--------|
| `Space` | Pause / resume |
| `↑` / `↓` | Nudge scroll position up / down |
| `←` / `→` | Decrease / increase scroll speed |
| `C` | Toggle Table of Contents |
| `Esc` | Stop and return to edit mode |

---

## Table of Contents

If your script uses Markdown-style headings, stp automatically generates a navigable table of contents.

```
# Section title        ← H1
## Subsection          ← H2
### Sub-subsection     ← H3
```

Open the TOC panel with **📋 TOC** or press `C`. Click any entry to jump directly to that section — scrolling continues from the new position. The panel closes automatically 5 seconds after a jump, or immediately when you click ✕.

The TOC panel slides in from the right without changing the width of your text.

---

## Mirror mode

Two independent mirror buttons:

- **↔ Horizontal** — flips text left-to-right, for reading via a teleprompter beamsplitter in front of a camera lens
- **↕ Vertical** — flips text upside-down

Both can be active simultaneously (180° rotation). The top bar is never affected.

---

## Tips

- **Speed**: start around 4–6 and use `←` / `→` to fine-tune while reading.
- **Width**: narrower (50–60%) reduces eye travel and feels more natural on large screens.
- **Font size**: go larger than you think you need — 40–52 px is comfortable at arm's length.
- **Markdown headings are optional** — plain text works fine; the TOC button is disabled when no headings are found.
