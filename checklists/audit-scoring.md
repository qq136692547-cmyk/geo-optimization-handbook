# Audit Scoring System

Based on the Auriti-Labs GEO Optimizer 8-dimension scoring framework.

---

## Score Card (100 Points Total)

| Category | Max Score | Your Score | Notes |
|----------|-----------|------------|-------|
| **Robots.txt** | 18 | | |
| **llms.txt** | 18 | | |
| **Schema JSON-LD** | 16 | | |
| **Meta Tags** | 14 | | |
| **Content** | 12 | | |
| **Brand & Entity** | 10 | | |
| **Signals** | 6 | | |
| **AI Discovery** | 6 | | |
| **Total** | **100** | | |

---

## Detailed Scoring Criteria

### Robots.txt (18 pts)

| Criteria | Points |
|----------|--------|
| OAI-SearchBot allowed | 3 |
| PerplexityBot allowed | 3 |
| ClaudeBot allowed | 3 |
| Google-Extended allowed | 3 |
| GPTBot disallowed | 3 |
| anthropic-ai disallowed | 3 |

### llms.txt (18 pts)

| Criteria | Points |
|----------|--------|
| llms.txt exists at root | 6 |
| Has H1 + blockquote structure | 4 |
| Has at least 2 area sections | 4 |
| Has descriptive links | 2 |
| Under 200 lines | 2 |

### Schema JSON-LD (16 pts)

| Criteria | Points |
|----------|--------|
| Organization schema present | 4 |
| Article schema on blog posts | 4 |
| FAQPage schema on Q&A content | 4 |
| 5+ properties populated per schema | 4 |

### Meta Tags (14 pts)

| Criteria | Points |
|----------|--------|
| og:title present and unique | 3 |
| og:description present (120-160 chars) | 3 |
| twitter:card present | 2 |
| Canonical URL set | 3 |
| HTML lang attribute correct | 3 |

### Content (12 pts)

| Criteria | Points |
|----------|--------|
| H1 present and descriptive | 2 |
| Content ≥ 800 words (blogs) | 2 |
| Statistics cited with sources | 2 |
| Clear heading hierarchy | 2 |
| Lists or tables present | 2 |
| External authoritative citations | 2 |

### Brand & Entity (10 pts)

| Criteria | Points |
|----------|--------|
| Consistent brand name across pages | 3 |
| About page with details | 2 |
| Contact information available | 2 |
| sameAs links in Organization schema | 3 |

### Signals (6 pts)

| Criteria | Points |
|----------|--------|
| HTML lang attribute matches content language | 2 |
| RSS/Atom feed available | 2 |
| Content freshness (recent updates) | 2 |

### AI Discovery (6 pts)

| Criteria | Points |
|----------|--------|
| .well-known/ai.txt endpoint | 2 |
| /ai/summary.json endpoint | 2 |
| /ai/faq.json endpoint | 2 |

---

## Scoring Levels

| Score | Level | Meaning |
|-------|-------|---------|
| 86–100 | Excellent | Fully GEO-optimized |
| 68–85 | Good | Minor gaps remain |
| 36–67 | Basic | Foundation exists, significant work needed |
| 0–35 | Critical | Major overhaul required |

---

## Automated Audit

For a fully automated audit, use the [Auriti-Labs GEO Optimizer](https://github.com/Auriti-Labs/geo-optimizer-skill):

```bash
pip install geo-optimizer-skill
geo audit --url https://yoursite.com
geo audit --sitemap https://yoursite.com/sitemap.xml --max-urls 25
```