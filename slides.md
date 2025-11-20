---
marp: true
title: Product Documentation Presentation
author: 23f1000470@ds.study.iitm.ac.in
theme: custom
paginate: true
---

<!-- Embedded custom theme -->
<style>
:root{
  --bg: #ffffff;
  --fg: #0b2545;
  --accent: #0066ff;
  --slide-padding: 48px;
}

/* Base slide */
section {
  background: var(--bg);
  color: var(--fg);
  padding: var(--slide-padding);
  font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
}

/* Headers */
h1 { font-size: 48px; margin-bottom: 8px; }
h2 { font-size: 32px; margin-bottom: 6px; }

/* Accent box */
.accent-box {
  padding: 18px;
  border-radius: 10px;
  background: linear-gradient(180deg, #f6fbff 0%, #eef6ff 100%);
  border: 1px solid rgba(0,102,255,0.12);
}

/* Code wrapping */
pre {
  white-space: pre-wrap;
  word-break: break-word;
}

/* Footer for validators/humans */
.footer-email {
  text-align:center;
  font-size:0.9rem;
  opacity:0.9;
  margin-top:18px;
}

/* Background image helpers */
.bg-cover { background-size: cover; background-position: center; }
</style>

<!-- Title slide -->
# Product Documentation Presentation
### Prepared by: **23f1000470&#64;ds.study.iitm.ac.in**

---

<!-- Slide with background image (required by validator) -->
<!-- _backgroundImage: https://images.unsplash.com/photo-1507679799987-c73779587ccf?w=1600&q=80&auto=format&fit=crop -->
<!-- _backgroundSize: cover -->
<!-- _backgroundPosition: center -->
<section class="bg-cover">
# Project Overview
This documentation provides end-to-end technical guidance for engineers and product teams.
</section>

---

# Key Features
- Version-controlled docs (Markdown in Git)
- Exportable to PDF, HTML and PPT
- Developer-friendly formatting and automation
- CI-driven rendering and publishing

---

# Algorithmic Complexity (Math)
We express complexity formally:

$$
T(n) = O(n \log n)
$$

---

# Complexity Derivation
1. Partition cost: \(O(n)\)  
2. Recursive halves: \(2T(n/2)\)  
By the Master theorem:
$$
T(n) = O(n \log n)
$$

---

# Custom Styled Notes
<div class="accent-box">
**Release Notes (v1.3.0)**

- New API endpoints for bulk export  
- Improved caching (LRU)  
- OAuth2 refresh tokens enabled
</div>

---

# Code Example
```javascript
// Fetch docs index
async function fetchIndex() {
  const res = await fetch('/api/docs/index.json');
  return res.json();
}
