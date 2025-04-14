---
title: Raspberry Pi Website Audit
layout: default
---

# 🧪 Raspberry Pi Website Audit

## Issues Found

### 1. Large JavaScript Payload

**File:** `web-component.js` (18MB)  
**Impact:** Delays interactivity, bad for mobile performance  
**Solution:** Lazy-load or defer this script unless editor is needed

### 2. Non-Compliant Cookie Consent

**Issue:** `_ga` cookie is set before consent  
**Solution:** Implement a GDPR-compliant CMP with granular controls

### 3. Image Optimization

**Issue:** Large unoptimized images  
**Solution:** Use `gatsby-plugin-image` for responsive, lazy-loaded images

---

## 💡 Recommendations

- Lazy-load non-critical JS (editor, analytics)
- Add a cookie consent banner with opt-in toggles
- Optimize image delivery using Gatsby tools
