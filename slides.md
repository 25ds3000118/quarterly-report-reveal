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
    opacity: 0.9;
  }
  .footnote {
    font-size: 0.75rem;
    opacity: 0.7;
  }
  .complexity { font-weight: 700; font-size: 1.1rem; }
---

<!-- _class: title-slide -->
# Quarterly Product Documentation

**Maintained in Markdown — easy to version, diff and convert.**

<span class="email">Email: 25ds3000118@ds.study.iitm.ac.in</span>

---

<!-- backgroundImage: url('./image/product-hero.jpg') -->
<!-- backgroundSize: cover -->
<!-- backgroundPosition: center -->

# Architecture Snapshot

This slide uses *product-hero.jpg* from your **image** folder as the background.

---

# Goals for this documentation

- Keep sources in plain Markdown for VCS friendliness.
- Produce PDF/HTML/Slides from the same source.
- Use directives and small CSS for consistent branding.

---

# How to build / preview

Use Marp CLI locally:

```bash
# install if you don't have it
npm i -g @marp-team/marp-cli

# preview locally
marp --html --allow-local-files slides.md -o slides.html
