# Mardakhay Ravinov — Resume Website

A clean, minimal personal resume website built with plain HTML and CSS. No frameworks, no dependencies, no build tools.

## Stack

- HTML5 (semantic elements)
- CSS3 (custom properties, grid, flexbox)
- Google Fonts — DM Serif Display + DM Sans

## Structure

```
index.html   ← the entire site, single file
README.md     ← this file
```

## Sections

- **Experience** — work history at ABB and AzeriMed
- **Education** — M.Sc and B.Sc from ASOIU
- **Skills** — technical skills and spoken languages
- **Projects** — personal projects with GitHub links
- **Licenses & Certifications** — 14 certificates from Codecademy, Google, and others

## How to run

Just open `index.html` in any browser. No server needed.

## How to update content

All content lives directly in `index.html`. Common updates:

**Add a skill:**
```html
<span class="skill-tag" role="listitem">Your Skill</span>
```

**Add a job:**
```html
<article class="exp-item">
  <h2 class="exp-role">Role — Company</h2>
  <div class="exp-date">Month Year – Month Year</div>
  <ul class="bullets">
    <li>What you did.</li>
  </ul>
</article>
```

**Add a project:**
```html
<article class="project-card">
  <div class="project-header">
    <h2 class="project-name">Project Name</h2>
    <div class="project-links">
      <a href="https://github.com/..." target="_blank" rel="noopener noreferrer">GitHub ↗</a>
    </div>
  </div>
  <p class="project-desc">What the project does in 1–2 sentences.</p>
  <div class="project-tags">
    <span class="project-tag">HTML5</span>
    <span class="project-tag">CSS3</span>
  </div>
</article>
```

**Add a certificate:**
```html
<article class="cert-card">
  <h3 class="cert-name">Certificate Name</h3>
  <p class="cert-issuer">Issuing Organization</p>
  <p class="cert-meta">Issued Mon YYYY · ID: XXXXXXXX</p>
  <div class="cert-skills"><span class="cert-skill">Skill</span></div>
</article>
```

## Design tokens

All colors and fonts are defined as CSS variables at the top of the `<style>` block:

```css
:root {
  --cream:      #f7f5f0;  /* background */
  --ink:        #1a1a18;  /* primary text */
  --muted:      #888880;  /* labels, dates */
  --subtle:     #555550;  /* body text */
  --line:       #ddddd5;  /* borders */
  --accent:     #c8593a;  /* terracotta highlight */
}
```
