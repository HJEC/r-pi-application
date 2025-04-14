---
title: ""
layout: ""
---

# 👋 Hi There!
Thanks for following the link to my super-special website audit that I put together for you

## What is this?
I wanted to convey just how enthusiastic I am about applying for the position of "Software Engineer at Raspberry-Pi". My way of showing this was to present what I'm bringing to the table. Not just technical skills, but enthusiasm and dedication. A willingness to go above and beyond. 

Whilst doing my research on the job position and the company, I did some digging and dev-sleuthing on the raspberry-pi websites. I've created a personal presentation for you based on some of the things I've found.

**Please read:** Before I continue, I would like to state that I never intended to step on anyone's toes with the information I am about to present. It should not be taken as harsh criticism or a judgement of any kind. I entrust that the good people already working on the sites at Raspberry-Pi (that I hope to join the ranks of) are doing an incredible job. This audit is just my attempt an enthusiastic attempt to put myself ahead of the competition!

## Nice enthusiasm! That sounds great, can you sum-it up?
I've broken down my findings into the following categories:
- Minor Issues (HTML/Styling)
- Notable Issues (Performance)

With each finding I will present my understanding of the issue, and my own recommended suggestion.




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
