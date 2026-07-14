# ArteDiStrada — Hero sections (two concepts)

Two alternative, professional hero sections. Both keep the **BUILT FROM
NOTHING.** headline, the brand tokens (`--ink/--bone/--acid`), and an optional
brand-film modal — pick whichever you prefer.

### Concept A — `hero.html` — "The Living Mark"
Logo-forward and centered. The animated brand mark (logo loop) glows in the
concrete void as the focal point; compact, editorial corner framing; **Watch
the story** button opens the film in a cinematic modal.

### Concept B — `hero-film.html` — "The Film"
Cinematic and asymmetric. The brand film plays as a darkened full-bleed
background (muted loop, like a fashion-film teaser); huge headline anchored
bottom-left; vertical side labels; a floating **Now Playing — Watch** pill and
a **Watch the full story** CTA both open the film with sound.

## Files
- `hero.html` — Concept A (self-contained HTML + CSS + JS).
- `hero-film.html` — Concept B (self-contained HTML + CSS + JS).
- `assets/logo-loop.mp4` — the seamless logo loop (centerpiece of Concept A).
- `assets/brand-video.mp4` — the story film (modal in both; background in Concept B).

## Preview
Open `hero.html` in a browser. The videos load from `assets/` next to the file.

## Add it to your existing site
1. Copy the two files from `assets/` into your site's media/assets folder.
2. Paste the `<section class="hero …>` … `</section>` block **and** the
   `#video-modal` block from `hero.html` into your page where the hero should go.
3. Copy the `<style>` block into your CSS (or keep it in the page `<head>`).
   The tokens `--ink / --bone / --acid` already match your site.
4. Copy the `<script>` block (dust, live counter, video modal) before `</body>`.
5. Fix the two `src="assets/…"` paths to wherever your videos live.

## Notes
- The logo loop is expected to be authored on a dark ground so it melts into
  the `--ink` stage; a feathered edge mask hides any hard video edges either
  way. If your loop has a light background, remove the `mask` lines on
  `.mark-video`.
- Respects `prefers-reduced-motion`. Modal closes on ✕, click-outside, or Esc.
- The `Shop the drop` button links to `#shop` — point it at your real shop URL.
