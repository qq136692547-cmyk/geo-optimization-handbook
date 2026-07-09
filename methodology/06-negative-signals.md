# Negative Signals

Based on UC Berkeley EMNLP 2024 research and Auriti-Labs GEO Optimizer. AI engines detect these signals and reduce your content's citation priority.

---

## The 8 Negative Signals

### 1. Excessive CTA Density
**Detection:** >5 CTAs or >1% of words are call-to-action language
**Fix:** Reduce self-promotional language. Keep a 90/10 ratio of informative to promotional content.

### 2. Popup/Modal Interference
**Detection:** Modal, overlay, lightbox, or popup elements
**Fix:** Minimize intrusive popups. Use banner-style CTAs instead.

### 3. Thin Content
**Detection:** <300 words with H1 promising depth
**Fix:** Match content length to heading promise. A detailed H1 needs 800+ words of real content.

### 4. Broken Links
**Detection:** >3 empty or invalid links
**Fix:** Regular link audits. Use a broken link checker monthly.

### 5. Keyword Stuffing
**Detection:** Single keyword density >2.5% with 5+ occurrences
**Fix:** Write naturally. Use synonyms and related terms.

### 6. Missing Author Signal
**Detection:** No Person schema or rel=author on content pages
**Fix:** Always include author byline with Person schema markup.

### 7. Excessive Boilerplate
**Detection:** Non-content text (nav, footer, sidebar) exceeds content in proportion
**Fix:** Keep navigation concise. Use minimal footers. Prioritize content area.

### 8. Mixed Signals
**Detection:** H1 promises depth but content is shallow
**Fix:** Ensure every H1/H2 promise is fulfilled in the following content.

---

## Severity Levels

| Classification | Signal Count | Action Required |
|----------------|-------------|-----------------|
| **High** | 4+ signals | Major overhaul needed |
| **Medium** | 2–3 signals | Targeted fixes |
| **Low** | 1 signal | Minor adjustment |

---

## Self-Audit Checklist

Run this on any page you want AI engines to cite:

- [ ] CTA count ≤ 5
- [ ] No intrusive popups
- [ ] Content ≥ 800 words for blog posts
- [ ] All links valid (0 broken)
- [ ] Primary keyword density < 2.5%
- [ ] Author byline + Person schema present
- [ ] Content-to-boilerplate ratio > 60%
- [ ] H1 promise matches content depth