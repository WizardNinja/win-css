# WiN-CSS

A mobile-first CSS framework with proportionally-scaling typography and spacing.

**[Documentation](https://wizardninja.github.io/win-css/)**

## The Idea

WiN-CSS uses **vw-based fonts** and **em-based spacing** so that text and padding/margin scale together proportionally. This means:

- Line breaks stay consistent across screen sizes
- Designs maintain their visual proportions
- Less manual tweaking at each breakpoint

At the `lg` breakpoint (1300px), fonts lock to fixed `px` values and `.row` gets a max-width, preventing content from scaling infinitely on large screens.

## Installation

**CDN**
```html
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/wizardninja/win-css@main/dist/win.css">
```

**npm**
```bash
npm install win-css
```

**Download**

Grab `dist/win.css` from this repo.

## Quick Start

```html
<div class="row">
  <div class="sm-12 md-6 lg-4 sm-p-10">
    <h2 class="sm-f-large md-f-xlarge sm-m-0 sm-my-10">Title</h2>
    <p class="sm-f-medium sm-m-0">Content that scales proportionally.</p>
  </div>
</div>
```

## Class Patterns

| Feature | Pattern | Example |
|---------|---------|---------|
| Grid | `{bp}-{1-12}` | `sm-12 md-6 lg-4` |
| Font size | `{bp}-f-{size}` | `sm-f-medium md-f-large` |
| Padding | `{bp}-p-{n}` | `sm-p-10 md-p-20` |
| Margin | `{bp}-m-{n}` | `sm-m-0 sm-my-15` |
| Aspect ratio | `{bp}-ar-{ratio}` | `sm-ar-16x9` |

**Breakpoints:** `sm` (360px), `md` (760px), `lg` (1300px)

**Spacing scale:** 0, 5, 10, 15, 20, 25, 30, 40, 50 (in tenths of em)

**Font sizes:** tiny, small, medium, large, xlarge, huge

## License

MIT
