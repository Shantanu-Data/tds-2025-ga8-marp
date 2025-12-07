---
marp: true
theme: product-docs
paginate: true
_paginate: true
title: Product Documentation Presentation
description: "Marp-based product documentation deck"
---

<style>
/* @theme product-docs */

/* Global typography and colors */
section {
  font-family: system-ui, -apple-system, BlinkMacSystemFont, "Segoe UI",
    sans-serif;
  background-color: #050816;
  color: #e5e7eb;
  padding: 2.5rem 3rem;
}

h1, h2, h3 {
  color: #fbbf24;
  letter-spacing: 0.03em;
}

/* Code blocks */
code, pre {
  font-family: "JetBrains Mono", Menlo, Monaco, Consolas, "Liberation Mono",
    "Courier New", monospace;
  background-color: #020617;
  border-radius: 0.4rem;
}

/* Highlighted slide class via Marp directive _class: highlight */
section.highlight {
  border-left: 8px solid #fbbf24;
  box-shadow: 0 0 0 1px #4b5563;
}

/* Footer text styling */
footer {
  font-size: 0.65rem;
  color: #9ca3af;
}

/* Page numbers (bottom-right) using Marp pagination data attributes */
section::after {
  position: absolute;
  right: 1.8rem;
  bottom: 1.2rem;
  font-size: 0.7rem;
  color: #9ca3af;
  content: attr(data-marpit-pagination) " / " attr(data-marpit-pagination-total);
}
</style>

<!-- _footer: "Product Docs – Internal • Marp Presentation" -->

# Product Documentation Overview

**Role:** Technical Writer, Platform Team

**Email:** **23f3002617@ds.study.iitm.ac.in**

- Maintainable, version-controlled documentation
- Single Markdown source → multiple output formats (HTML, PDF, PPTX)
- Built with **Marp** and stored in **Git**

---

<!-- _class: highlight -->
<!-- _footer: "Why Marp for product documentation?" -->

## Why Marp for Product Docs?

- Documentation lives in **version control (Git)**  
- Writer-friendly **Markdown** syntax  
- Can be **reviewed via Pull Requests**  
- Easily converted to:
  - HTML slides for internal demos
  - PDF decks for customers
  - PPTX for executives

> One source of truth, multiple distribution formats.

---

<!-- Background image slide -->
<!-- _backgroundImage: "url('https://images.unsplash.com/photo-1553877522-43269d4ea984?auto=format&fit=crop&w=1600&q=80')" -->
<!-- _backgroundSize: cover -->
<!-- _backgroundColor: "#000000cc" -->
<!-- _footer: "System architecture – high-level view" -->

# Architecture at a Glance

- API Gateway
- Authentication & Authorization service
- Documentation Rendering service (Marp CLI)
- Object storage (release artifacts)

---

<!-- _footer: "Custom theme & directives in Marp" -->

## Custom Theme & Marp Directives

This deck uses a **custom theme**:

- Defined in the same file via CSS:

```css
/* @theme product-docs */
section {
  background-color: #050816;
  color: #e5e7eb;
}
