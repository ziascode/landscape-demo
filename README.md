# TongHui Landscaping: website redesign concept

A redesign concept for [TongHui Landscaping](https://tonghuilandscaping.ca) (Toronto & GTA). **This is not the company's live website.**

The concept is "laid stone by stone": the hero photo assembles itself from herringbone pavers, the way an interlocking driveway is actually built.

## What's in it

- **Paver hero:** a canvas animation lays the hero photo brick by brick in a herringbone pattern.
- **Before & after slider:** drag, touch or keyboard, built from the company's own before/after photos.
- **Services:** on desktop, scrolling moves a horizontal track. On phones it becomes a native swipe rail.
- **Workflow:** five steps, with a paver-path progress indicator that follows the step in view.
- **Project gallery** with a full-screen lightbox (arrows, swipe, Esc).
- **Contact form** that opens the visitor's email app with the request filled in, plus a sticky call bar on phones.
- **Logo:** an HD vector redraw of the original (`assets/logo.svg`, `assets/logo-hd.png`).

Built with plain HTML, CSS and JavaScript, using [GSAP](https://gsap.com) + ScrollTrigger and [Lenis](https://lenis.darkroom.engineering) from CDNs. There is no build step.

## Run it locally

Some browsers block local files, so serve the folder:

```bash
python3 -m http.server 8000
```

Then open http://localhost:8000.

## Notes

- Project photos load from the company's current site (tonghuilandscaping.ca/images/). A production version should copy them into `assets/` and compress them.
- `assets/hero-hd.jpg` is a 2× upscale of the original 1200×800 hero photo (`assets/hero-original.jpg`).
- The contact form uses `mailto:`. A production version needs a form backend.
