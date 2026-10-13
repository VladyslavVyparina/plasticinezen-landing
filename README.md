# PlasticineZen landing

A single-page course landing page built to drop into a SendPulse HTML block, with a lesson sample and a thank-you page.

## Problem

The course needed a page that listed the program, showed a sample lesson, and collected a purchase, and the mailing tool in use only accepts an HTML block plus files you host yourself.

## What was built

- `index.html` is one document: sections and styles together, ready to paste into SendPulse.
- `images/` holds the logo, the hero polaroid, the program header, and material photos.
- `videos/pryklad-uroku.mp4` is the sample lesson, played with a plain HTML5 player. Host that folder next to the HTML.
- `thank-you.html` is the page after the form.
- `form.html` and the `sendpulse-*.js` files are the form and the thank-you behavior split out for the mailing tool.
- `email-templete.html` is the matching email layout.

## How it works

The page is static. Purchase buttons are `href="#"` until a real LiqPay or SendPulse payment URL is pasted in. The Instagram link in the footer is a placeholder the same way. Nothing on the page calls a backend in this repository.

## Stack

HTML, CSS, JavaScript.

## Run locally

Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8080
```

## Before publishing the page

Replace the Instagram URL and point every buy button at the real checkout. Upload `videos/` with the HTML.
