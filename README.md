# Hero — "The Living Mark"

A new, logo-forward hero section for ArteDiStrada. No product cards — the
first thing a visitor sees is the animated brand mark glowing in the concrete
void, the **BUILT FROM NOTHING.** headline, and a **Watch the story** button
that opens the brand film in a cinematic modal (optional — nobody's forced to
watch it).

## Files
- `hero.html` — the full, self-contained hero (HTML + CSS + JS in one file).
- `assets/logo-loop.mp4` — the seamless logo loop (plays muted/looping as the centerpiece).
- `assets/brand-video.mp4` — the story film (opens in the modal on click).

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
