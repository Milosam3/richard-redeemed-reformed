```markdown
# Richard Redeemed Reformed — site reference

## Key details

| Item | Detail |
|---|---|
| Live site | https://richardredeemedreformed.co.za |
| GitHub repository | github.com/milosam3/richard-redeemed-reformed |
| GitHub Pages URL | milosam3.github.io/richard-redeemed-reformed |
| Domain registrar | Afrihost — afrihost.co.za |
| Hosting | GitHub Pages (free) |
| Contact form | Formspree — formspree.io (update YOUR_FORM_ID in contact.html) |

---

## How to publish a new post

1. Write and finish your post in Google Docs. Note the title and write a one or two sentence excerpt.
2. Go to your GitHub repository → posts folder → open post-template.html → click pencil icon → select all code and copy it.
3. Go back to posts folder → Add file → Create new file. Name it using lowercase and hyphens e.g. `posts/my-post-title.html`
4. Paste the copied code. Update the title tag, post-date, page-title heading, and paste each paragraph from Google Docs into its own `<p>` tag inside page-body.
5. Scroll down and click Commit new file.
6. Open index.html → click edit → add a new post row at the top of the recent writing section → commit.
7. Do the same in writing.html → commit.
8. Wait one minute then visit richardredeemedreformed.co.za and click your post to confirm it loads.
9. Share a punchy two or three line excerpt on X with a link back to the full post.

### Post row to copy into index.html and writing.html

```html
<div class="post-row">
  <p class="post-date">March 2026</p>
  <p class="post-title"><a href="posts/your-filename.html">Your title</a></p>
  <p class="post-excerpt">One or two sentence summary.</p>
</div>
```

---

## Security

- Your site is static HTML with no database — almost nothing to attack. Very safe.
- HTTPS is enabled — all traffic is encrypted.
- Content cannot be changed unless someone accesses your GitHub account. Enable two-factor authentication (2FA) in GitHub Settings → Password and authentication.
- Hosted on GitHub Pages (Microsoft infrastructure) — extremely reliable.
- Complete your Formspree setup — replace YOUR_FORM_ID in contact.html with your actual ID from formspree.io.
- Your HTML source code is publicly visible — this is normal. Never put passwords or personal ID numbers in your files.

---

## File structure

```
richard-redeemed-reformed/
├── CNAME
├── style.css
├── index.html
├── writing.html
├── contact.html
├── logo.html
├── logos.html
└── posts/
    ├── post-template.html
    └── [your posts go here]
```

---

## CNAME

```
richardredeemedreformed.co.za
```

---

## style.css

```css
* { box-sizing: border-box; margin: 0; padding: 0; }
body {
  font-family: Georgia, 'Times New Roman', serif;
  background: #111111;
  color: #d4d0c8;
  font-size: 16px;
  line-height: 1.7;
}
a { color: inherit; text-decoration: none; }
.site { max-width: 680px; margin: 0 auto; padding: 2rem 1.5rem; }
nav {
  display: flex;
  justify-content: space-between;
  align-items: flex-start;
  padding-bottom: 2rem;
  border-bottom: 1px solid #2a2a2a;
  margin-bottom: 3rem;
}
.nav-links { display: flex; gap: 24px; padding-top: 8px; }
.nav-links a { font-size: 13px; color: #666; }
.nav-links a:hover { color: #d4d0c8; }
.hero { margin-bottom: 3rem; }
.hero-label {
  font-size: 11px;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: #555;
  margin-bottom: 1rem;
}
.hero-title {
  font-size: 30px;
  font-weight: 400;
  line-height: 1.3;
  margin-bottom: 1.25rem;
  color: #e8e4dc;
}
.hero-sub {
  font-size: 15px;
  color: #888;
  max-width: 520px;
  line-height: 1.8;
}
hr.divider {
  border: none;
  border-top: 1px solid #2a2a2a;
  margin: 2.5rem 0;
}
.section-label {
  font-size: 11px;
  letter-spacing: 0.12em;
  text-transform: uppercase;
  color: #555;
  margin-bottom: 1.5rem;
}
.post-row {
  padding: 1.25rem 0;
  border-bottom: 1px solid #2a2a2a;
}
.post-row:first-of-type { border-top: 1px solid #2a2a2a; }
.post-date { font-size: 12px; color: #555; margin-bottom: 4px; }
.post-title {
  font-size: 17px;
  font-weight: 400;
  line-height: 1.4;
  margin-bottom: 6px;
  color: #d4d0c8;
}
.post-title a:hover { text-decoration: underline; }
.post-excerpt { font-size: 13px; color: #666; line-height: 1.7; }
.page-title {
  font-size: 26px;
  font-weight: 400;
  margin-bottom: 1rem;
  color: #e8e4dc;
}
.page-body { font-size: 15px; color: #888; line-height: 1.9; max-width: 560px; }
.page-body p { margin-bottom: 1.25rem; }
.contact-form { max-width: 480px; margin-top: 2rem; }
.form-group { margin-bottom: 1.25rem; }
label { display: block; font-size: 13px; color: #666; margin-bottom: 6px; }
input, textarea {
  width: 100%;
  padding: 10px 12px;
  border: 1px solid #2a2a2a;
  font-family: Georgia, serif;
  font-size: 14px;
  color: #d4d0c8;
  background: #1a1a1a;
  border-radius: 4px;
}
input:focus, textarea:focus { outline: none; border-color: #555; }
textarea { height: 120px; resize: vertical; }
button[type="submit"] {
  padding: 10px 24px;
  background: #d4d0c8;
  color: #111;
  border: none;
  font-family: Georgia, serif;
  font-size: 14px;
  cursor: pointer;
  border-radius: 4px;
}
button[type="submit"]:hover { background: #e8e4dc; }
.footer {
  margin-top: 4rem;
  padding-top: 1.5rem;
  border-top: 1px solid #2a2a2a;
  font-size: 12px;
  color: #444;
}
```

---

## posts/post-template.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Post Title — Richard Redeemed Reformed</title>
  <link rel="stylesheet" href="../style.css">
</head>
<body>
<div class="site">
  <nav>
    <a href="../index.html" style="display:inline-block; line-height:0;">
    <svg width="110" height="140" viewBox="0 0 280 360" xmlns="http://www.w3.org/2000/svg">
      <path d="M75,235 Q140,218 140,218 Q140,218 205,235 L205,285 Q140,268 140,268 Q140,268 75,285 Z" stroke="#d4d0c8" stroke-width="1.5" fill="none"/>
      <line x1="140" y1="218" x2="140" y2="285" stroke="#d4d0c8" stroke-width="1"/>
      <line x1="86" y1="243" x2="138" y2="230" stroke="#888" stroke-width="0.8"/>
      <line x1="86" y1="253" x2="138" y2="240" stroke="#888" stroke-width="0.8"/>
      <line x1="86" y1="263" x2="138" y2="250" stroke="#888" stroke-width="0.8"/>
      <line x1="86" y1="273" x2="138" y2="260" stroke="#888" stroke-width="0.8"/>
      <line x1="194" y1="243" x2="142" y2="230" stroke="#888" stroke-width="0.8"/>
      <line x1="194" y1="253" x2="142" y2="240" stroke="#888" stroke-width="0.8"/>
      <line x1="194" y1="263" x2="142" y2="250" stroke="#888" stroke-width="0.8"/>
      <line x1="194" y1="273" x2="142" y2="260" stroke="#888" stroke-width="0.8"/>
      <line x1="140" y1="110" x2="140" y2="255" stroke="#e8e4dc" stroke-width="4.5"/>
      <line x1="106" y1="143" x2="174" y2="143" stroke="#e8e4dc" stroke-width="4.5"/>
      <line x1="90" y1="308" x2="190" y2="308" stroke="#333" stroke-width="0.8"/>
      <text x="140" y="298" font-family="Georgia, serif" font-size="11" fill="#666" text-anchor="middle" letter-spacing="5">RICHARD</text>
      <text x="140" y="324" font-family="Georgia, serif" font-size="14" fill="#e8e4dc" text-anchor="middle" letter-spacing="3">REDEEMED</text>
      <text x="140" y="342" font-family="Georgia, serif" font-size="14" fill="#e8e4dc" text-anchor="middle" letter-spacing="3">REFORMED</text>
    </svg>
    </a>
    <div class="nav-links">
      <a href="../index.html">Home</a>
      <a href="../writing.html">Writing</a>
      <a href="../contact.html">Contact</a>
    </div>
  </nav>
  <p class="post-date">March 2026</p>
  <h1 class="page-title">Your post title here</h1>
  <hr class="divider">
  <div class="page-body">
    <p>First paragraph.</p>
    <p>Second paragraph.</p>
  </div>
  <div class="footer">
    &copy; 2026 Richard Redeemed Reformed
    &nbsp;&mdash;&nbsp;
    <a href="../writing.html">Back to writing</a>
  </div>
</div>
</body>
</html>
```

---

*Last updated March 2026*
```

