# Structured Data for GEO

Structured data (JSON-LD schema markup) is one of the highest-ROI GEO tactics. Correct schema markup can improve AI extraction accuracy from **16% to 54%** (Semrush).

---

## FAQPage Schema (Highest ROI)

FAQPage schema is the most frequently used schema by AI search engines. AI models often extract Q&A pairs from FAQPage markup to answer user questions.

### When to Use

- Any page with question-answer content
- Blog posts covering"How to" topics
- Product pages with common questions
- Documentation with troubleshooting sections

### Template

```json
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "FAQPage",
  "mainEntity": [
    {
      "@type": "Question",
      "name": "What is the TikTok Shop commission rate in 2026?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "The TikTok Shop referral fee is 6% per transaction for all categories as of 2026. This is a flat rate that replaced the earlier category-based structure."
      }
    },
    {
      "@type": "Question",
      "name": "How does TikTok Shop compare to Amazon FBA fees?",
      "acceptedAnswer": {
        "@type": "Answer",
        "text": "TikTok Shop charges a flat 6% referral fee. Amazon FBA fees include referral fees (8-15% by category), fulfillment fees ($3-$6 per unit), and storage fees ($0.75-$2.40 per cubic foot monthly)."
      }
    }
  ]
}
</script>
```

### Rules for AI-Friendly Q&A

- **Questions** = real search queries users type (check Search Console for actual queries)
- **Answers** = 40–80 words, self-contained (no "as mentioned above")
- Each Q&A must work as a standalone answer
- Include specific numbers when possible
- 3–10 Q&A pairs per page
- **Must match visible content** — don't put questions in schema that aren't answered in the visible page

---

## Article Schema

### Template

```json
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Article",
  "headline": "TikTok Shop Fees vs Amazon FBA: Complete 2026 Comparison",
  "author": {
    "@type": "Person",
    "name": "L.D. Studio",
    "url": "https://example.com/about"
  },
  "datePublished": "2026-07-01",
  "dateModified": "2026-07-10",
  "description": "Compare TikTok Shop and Amazon FBA fees for 2026. Commission rates, fulfillment costs, storage fees, and profit analysis for sellers."
}
</script>
```

### Why Author Schema Matters

Negative GEO signal #6 is **missing author signal**. AI engines check for Person schema or rel=author. Content without author attribution is less likely to be cited.

---

## Organization Schema

```json
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "Organization",
  "name": "Your Brand Name",
  "url": "https://example.com",
  "logo": "https://example.com/logo.png",
  "sameAs": [
    "https://github.com/your-org",
    "https://twitter.com/your-handle"
  ]
}
</script>
```

### Key Fields for GEO

| Field | Importance | Why |
|-------|-----------|-----|
| `name` | Required | Brand identification |
| `url` | Required | Canonical identity |
| `logo` | Recommended | Visual brand signal |
| `sameAs` | Recommended | Cross-platform authority |
| `description` | Recommended | Brand summary for AI extraction |
| `foundingDate` | Nice to have | Longevity signal |

---

## HowTo Schema

### When to Use

- Calculator tool pages
- Step-by-step guides
- Tutorial content
- Setup instructions

### Template

```json
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "HowTo",
  "name": "How to calculate your TikTok Shop profit",
  "step": [
    {
      "@type": "HowToStep",
      "text": "Enter your product price and cost. The calculator subtracts the 6% referral fee, shipping cost, and any promotional discounts."
    },
    {
      "@type": "HowToStep",
      "text": "Review the breakdown showing gross revenue, fees, net profit, and profit margin percentage."
    }
  ]
}
</script>
```

---

## Schema Placement

### Static HTML Sites

Insert JSON-LD in the `<head>` section just before `</head>`, or in the `<body>` just after the opening tag.

### Blogger/Blogspot

Insert JSON-LD **in the post body**, not the template head. Blogger's template system can't be modified per-post via API.

### WordPress

Use a plugin (Yoast SEO, Rank Math, Schema Pro) or insert via theme's `functions.php`.

---

## Schema Validation

Always validate your structured data:

- [Google Rich Results Test](https://search.google.com/test/rich-results)
- [Schema.org Validator](https://validator.schema.org/)

## Common Schema Mistakes

| Mistake | Fix |
|---------|-----|
| FAQPage schema without visible FAQ | Add visible `<details><summary>` FAQ matching the schema |
| Missing author in Article schema | Add Person or Organization author |
| Wrong @type for content type | Match schema type to actual content (FAQPage for Q&A, not Article) |
| FAQPage with 1 Q&A pair | Minimum 3 pairs for significant GEO impact |
| Schema in HTML but not matching visible text | Ensure schema content matches page content |
| No datePublished or dateModified | Always include both for Article schema |