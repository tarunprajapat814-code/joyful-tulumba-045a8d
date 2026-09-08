# Apna Vyapar Website

यह एक तेज़, responsive और search-engine-friendly Hindi business website है। इसे Netlify पर deploy करने और Google Search Console में submit करने के लिए तैयार किया गया है।

## मुख्य तकनीकें

- Semantic HTML5
- Custom responsive CSS
- Vanilla JavaScript
- Netlify Forms
- `robots.txt`, XML sitemap और structured data

## Local रूप से चलाना

Repository root से कोई भी static file server चलाएँ और `public` directory serve करें। उदाहरण:

```bash
npx serve public
```

Netlify features को locally emulate करने के लिए:

```bash
netlify dev --port 8889
```

## जरूरी customization

Public launch से पहले `Apna Vyapar` को असली business name से बदलें और homepage metadata, services, contact expectations तथा canonical URL को वास्तविक business details के अनुसार update करें। Custom domain जोड़ने पर `public/index.html`, `public/robots.txt` और `public/sitemap.xml` में Netlify URL बदलें।
