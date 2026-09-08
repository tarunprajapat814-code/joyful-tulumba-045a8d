# Project Guide

## Architecture

यह zero-build static Netlify site है। Deploy output सीधे `public/` directory से serve होता है। कोई frontend framework या package installation आवश्यक नहीं है।

## Key Directories

- `public/index.html`: Homepage content, SEO metadata, structured data और Netlify enquiry form
- `public/styles.css`: Design system, responsive layout और animations
- `public/script.js`: Mobile navigation और dynamic footer year
- `public/robots.txt`: Search crawler policy
- `public/sitemap.xml`: Search engine sitemap
- `netlify.toml`: Publish directory और security headers

## Conventions

- Visible copy Hindi में रखें और HTML attributes/identifiers English में रखें।
- Semantic HTML तथा keyboard accessibility बनाए रखें।
- Colors और typography को `styles.css` के root variables से बदलें।
- Performance के लिए JavaScript को minimal रखें और motion में केवल opacity/transform animate करें।
- Netlify Form का `name`, hidden `form-name` और सभी field names synchronized रखें।

## Non-obvious Decisions

Template fetch उपलब्ध न होने के कारण site को dependency-free static architecture में बनाया गया। इससे initial rendering तेज़ रहती है और crawler को पूरा content बिना JavaScript के मिलता है। Canonical URL अभी Netlify project URL है; custom domain मिलने पर सभी SEO URL references एक साथ बदलने चाहिए।
