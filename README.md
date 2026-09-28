# Project Belle — CreditSwan Intelligence Packet (v1.2, 29 Sep 2026)

Static site. No build step, no middleware. The password gate is inside index.html itself:
the packet is AES-256-GCM encrypted in the file and decrypts in the browser with the password (Belle2026).
The same file works opened locally.

Deploy
  npx vercel --prod          # from this folder; framework preset: Other; output directory: public
  or drag the folder onto vercel.com/new

Contents
  public/index.html   the password-gated packet (self-contained; fonts from Google Fonts)
  public/robots.txt   disallow all
  vercel.json         clean URLs, no-cache, noindex headers
