# evamacsai-site

Static marketing site for **Eva Macsai, WHNP** — a private GYN practice in Teaneck, NJ.

No build step, no templating — the files at the repo root are what gets served.

```
index.html        home: hero (headshot + "Send a text" CTA), welcome, services, closing
schedule.html     "Book a visit" — single text-to-book button
inquire.html      redirect → schedule.html
style.css         lavender/plum palette (brand color #913b82)
logo.png          brand mark (transparent)   · logo-full.png = master
headshot-round.png circular hero portrait     · headshot-full.png = master
favicon.svg  robots.txt  sitemap.xml  CNAME  .nojekyll
```

Booking is by text: the CTAs are `sms:` links to (201) 925-4846 with a prefilled message.

## Run locally

```bash
python3 -m http.server 8080   # then open http://localhost:8080
```

## Deploy

Hosted on **GitHub Pages** from `main` (root). Push to `main` and it redeploys
automatically. Custom domain `evamacsai.com` is set via the `CNAME` file +
Namecheap DNS; GitHub auto-provisions HTTPS.
