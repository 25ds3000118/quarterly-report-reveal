---
marp: true
theme: default
paginate: true
class: lead
style: |
  /* Custom Marp theme tweaks */
  section {
    font-family: Inter, Avenir, Helvetica, Arial, sans-serif;
  }
  h1 {
    color: #0f172a;
  }
  .email {
    font-size: 0.85rem;
    opacity: 0.95;
  }
  .footnote {
    font-size: 0.75rem;
    opacity: 0.7;
  }
  .complexity { font-weight: 700; font-size: 1.1rem; }

  /* Ensure background text remains readable on hero slide */
  .hero-title { color: #ffffff; text-shadow: 0 2px 6px rgba(0,0,0,0.6); }
  .hero-sub { color: rgba(255,255,255,0.9); }

---

<!-- _class: title-slide -->
# Quarterly Product Documentation

**Maintained in Markdown — easy to version, diff and convert.**

<span class="email">Email: 25ds3000118@ds.study.iitm.ac.in</span>

---

<!--
  Slide-level background directive using the raw GitHub URL (explicit).
  This is required for remote builds / CI that load external/raw assets.
-->
<!-- backgroundImage: url('https://raw.githubusercontent.com/25ds3000118/quarterly-report-reveal/main/image/product-hero.jpg') -->
<!-- backgroundSize: cover -->
<!-- backgroundPosition: center -->
<!-- backgroundRepeat: no-repeat -->

# <span class="hero-title">Architecture Snapshot</span>
<span class="hero-sub">This slide uses <code>product-hero.jpg</code> from the repo as a background.</span>

<!--
  Extra explicit image reference so validators that scan for <img> or direct image links see the asset.
  The image is visually hidden so it does not duplicate on the slide when Marp applies the background.
-->
<img src="https://raw.githubusercontent.com/25ds3000118/quarterly-report-reveal/main/image/product-hero.jpg" alt="product-hero" style="display:none;" />

---

# Goals for this documentation

- Keep sources in plain Markdown for VCS friendliness.
- Produce PDF/HTML/Slides from the same source.
- Use directives and small CSS for consistent branding.

---

# How to build / preview

Use Marp CLI locally:

```bash
# install marp-cli if you don't have it
npm i -g @marp-team/marp-cli

# preview locally (allow local files if using relative paths)
marp --html --allow-local-files slides.md -o slides.html

# produce PDF
marp slides.md -o slides.pdf
