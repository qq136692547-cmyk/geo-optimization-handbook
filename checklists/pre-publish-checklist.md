# Pre-Publish GEO Checklist

Run this checklist before publishing ANY blog post or article.

---

## 8-Item Checklist

### 🔲 1. Definitional Opening
First 100 words directly answer the core question — no fluff, no welcome message.

### 🔲 2. FAQ Section
- 3+ Q&A pairs at the end of the article
- Visible HTML section (not just JSON-LD)
- FAQPage JSON-LD schema matching the visible content

### 🔲 3. Cited Data
At least one specific statistic, percentage, or year with source attribution.

### 🔲 4. Author Attribution
Author byline present with Person schema (JSON-LD or rel=author).

### 🔲 5. External Authority Link
At least one link to .edu, .gov, or recognized industry authority.

### 🔲 6. Structured Content
Information organized in bullet lists or comparison tables.

### 🔲 7. Internal Links
Link to at least one related article or tool on the same site.

### 🔲 8. No Excessive CTAs
No consecutive promotional sentences. Keep 90/10 informative/promotional ratio.

---

## Negative Signal Check

Ensure NONE of these are present:

- [ ] No keyword stuffing (single keyword >2.5% density)
- [ ] No thin content (<800 words for blog posts, <300 for tool pages)
- [ ] No missing author attribution
- [ ] No broken external links
- [ ] No fabricated data or unverified claims
- [ ] No excessive popups or modals

---

## Technical Check

- [ ] robots.txt allows AI citation bots
- [ ] llms.txt deployed (if applicable)
- [ ] OG tags present with unique title/description
- [ ] Twitter card tags present
- [ ] Canonical URL set
- [ ] Page loads in <3 seconds

---

## Quick Audit Script

```bash
# Run from the article's directory
echo "=== Word count ==="
wc -w article.md

echo "=== FAQPage check ==="
grep -c 'FAQPage' article.html

echo "=== Author check ==="
grep -c 'By ' article.md

echo "=== External links ==="
grep -c 'http\|https' article.md

echo "=== CTA density ==="
grep -oi 'sign up\|subscribe\|buy now\|get started\|try free' article.md | wc -l
```