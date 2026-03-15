# Illinois Brand Compliance Audit

**Reference:** `illinois_brand_header_footer_audit.docx`  
**Reference site:** [siebelschool.dev.engr.illinois.edu/natural-language-processing](https://siebelschool.dev.engr.illinois.edu/natural-language-processing)

This checklist is aligned with the audit doc prepared for code-agent implementation. The guideline states that **illinois.edu sites must use the university’s standard web header and footer** and recommends **Illinois Web Toolkit components** or a very close implementation.

---

## 1. Executive summary

| Area | Status | Notes |
|------|--------|--------|
| **Colors** | ✅ Compliant | Illini Blue `#13294B` and Illini Orange `#FF5F05` used via CSS variables. |
| **Typography** | ✅ Compliant | Montserrat (headings/nav) and Source Sans Pro (body) per brand guidelines. |
| **CSS tokens** | ✅ Compliant | `--il-blue`, `--il-orange`, `--il-storm`, `--font-heading`, `--font-body` defined. |
| **Header structure** | ⚠️ Partial | Top bar has Grainger + Siebel School. Block I and utility strip optional for non-toolkit sites. |
| **Logo** | ⚠️ Verify | Use **official Block I** from [brand.illinois.edu](https://brand.illinois.edu/); link to illinois.edu. No custom unit logos. |
| **Footer** | ✅ Compliant | Contact, address, Explore/Connect, social, policy row (Privacy, Accessibility, Webmaster, Copyright). |
| **Accessibility** | ✅ Addressed | Landmarks, skip link, focus states, semantic HTML. Aim for WCAG 2.2. |

---

## 2. Required by Illinois brand guidance

### Header / footer
- **Requirement:** Use university’s standard web header and footer; prefer toolkit components.
- **Status:** Custom header/footer implemented to mirror reference structure (top bar, unit name, nav, footer with contact and policy links). For full compliance on illinois.edu, consider adopting the official Illinois Web Toolkit header/footer.

### Required header elements (minimum)
- Branding strap / Block I in Illini blue context  
- University of Illinois Urbana-Champaign text  
- Primary unit name; local site name as home  

**Current implementation:**  
- Top bar: “The Grainger College of Engineering” | “Siebel School of Computing and Data Science” (link to Siebel).  
- Main header: logo (ensure this is Block I per note below) + “NLP @ UIUC” (home) + “University of Illinois at Urbana-Champaign” in description.  
- **Action:** Confirm logo is the official Block I and that it links to illinois.edu when used as the main university mark. If the site is a sub-site, the “home” link may remain to the NLP site.

### Colors
- **Requirement:** Illini orange and Illini blue as dominant; use official hex.
- **Status:** ✅ `#13294B` (blue) and `#FF5F05` (orange) used throughout via tokens.

### Typography
- **Requirement:** Montserrat (headings/nav), Source Sans Pro (body), Georgia (quotes if needed).
- **Status:** ✅ Font stack uses Montserrat for headings and nav, Source Sans Pro for body.

### Logos
- **Requirement:** Block I is the official logo; no custom unit logos; do not redraw, distort, or combine with custom wordmarks.
- **Status:** ⚠️ **Verify** that `graphics/plain-logo.png` is the official Block I from [brand.illinois.edu](https://brand.illinois.edu/). If it is a custom NLP mark, replace with the Block I and link the Block I to illinois.edu per guidelines.

### Accessibility
- **Requirement:** WCAG 2.2; landmarks, contrast, focus, keyboard.
- **Status:** Skip link, `<header>`, `<nav>`, `<main>`, `<footer>`, focus styles in place. Continue to test with keyboard and screen reader.

---

## 3. CSS tokens (implementation spec)

Aligned with the audit doc:

| Token | Value | Use |
|-------|--------|-----|
| `--il-blue` | `#13294B` | Primary brand blue (header, emphasis) |
| `--il-orange` | `#FF5F05` | Accent, highlights |
| `--il-storm` | `#707372` | Secondary text, dividers |
| `--il-white` | `#FFFFFF` | Text on blue, backgrounds |
| `--font-heading` | Montserrat, sans-serif | Headlines, nav |
| `--font-body` | "Source Sans Pro", sans-serif | Body, UI |

Legacy names `--illini-blue` and `--illini-orange` are kept as aliases where needed.

---

## 4. Footer (reference structure)

Confirmed from audit doc; implemented on site:

- Siebel School / University of Illinois Urbana-Champaign  
- Thomas M. Siebel Center address, phone, email  
- Social links (Twitter, Instagram, Facebook, LinkedIn, YouTube)  
- **Explore:** Find People, Office Locations, (Events), University of Illinois  
- **Connect:** Graduate Advising, NLP Group contact  
- **Policy row:** Privacy Policy, Copyright © 2026, Accessibility, Webmaster  

Optional additions if desired: Chicago office block, Engineering IT, Office of Safety, Marketing and Communications (add when official URLs are provided).

---

## 5. Compliance risks to avoid (from audit doc)

- Using a custom header that only “looks close” instead of standard structure or toolkit.  
- Using near-match colors instead of official Illini Blue and Illini Orange.  
- Using the unit name as a custom logo or combining it with Block I in a non-standard way.  
- Dropping accessibility (focus, landmarks, keyboard, menu states).  
- Footer with only a copyright line and no institutional/policy links.  

---

## 6. Next steps (recommended)

1. **Logo:** Replace `graphics/plain-logo.png` with the official Block I from [brand.illinois.edu](https://brand.illinois.edu/) and link it to https://illinois.edu if it serves as the main university mark.  
2. **Toolkit:** If the site will live on illinois.edu, evaluate integrating the official Illinois Web Toolkit header and footer for full compliance.  
3. **Extraction workflow:** For pixel-perfect match to the reference page, use the audit doc’s extraction workflow (DevTools computed styles, breakpoints, accessibility checks) and adjust spacing/font-size as needed.

---

*Last updated from implementation and `illinois_brand_header_footer_audit.docx`.*
