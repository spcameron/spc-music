# spc-music

A personal writing site focused on music.

This site is built using:

- `press` — a small static site generator
- `scribe` — a Markdown compiler
- `templ` — HTML templating in Go
- Tailwind CSS — utility-first styling

---

## Development

### Build

```bash
just build-all
```

Builds:

- CLI binary
- CSS (Tailwind)
- static site output

### Serve (live reload)

```bash
just serve-live
```

Watches source files and rebuilds the site on change.

---

## Structure

```text
content/    markdown content (posts and pages)
templates/  templ components
static/     static assets (including compiled CSS)
```

The site is built into:

```text
build/public/
```

---

## Notes

- Styling is compiled from `static/css/tailwind.css` into `static/css/styles.css`, and only the compiled CSS is used by the site
