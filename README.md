# Farah & Mahmoud — Site Setup Checklist

## 1. Cover photo (WhatsApp / social preview) — done
`assets/cover.jpg` is ready to go (resized to 1200x1200 from your invitation image).

Once your site is live on GitHub Pages, open `index.html` and replace the two
placeholders with your real address:
- `https://YOUR-USERNAME.github.io/YOUR-REPO/assets/cover.jpg`
- `https://YOUR-USERNAME.github.io/YOUR-REPO/` (the og:url line)

WhatsApp caches previews aggressively — after publishing, test your real link at
https://developers.facebook.com/tools/debug/ and click "Scrape Again" if the
image doesn't show up right away.

## 2. Music
Waiting on the correct song file from you. Once you send it:
- Save it as `assets/music.mp4` (or `.mp3`) — the page already looks for both.
- Nothing else needs to change; the site auto-plays it (muted-safe, one tap to start)
  when a guest taps "Enter."

## 3. Guest photo upload (QR code)
`upload.html` is ready but needs YOUR Google Drive link plugged in:

1. Go to drive.google.com → New folder, e.g. "Farah & Mahmoud - Guest Photos."
2. Right-click the folder → **File request** (if you don't see it, use the
   "+" or "···" menu on the folder).
3. Name it (e.g. "Guest Photos") → Create.
4. Copy the link Drive gives you.
5. Open `upload.html`, find `YOUR_GOOGLE_DRIVE_FILE_REQUEST_LINK`, and paste
   your link in its place (there's one spot, in the button's `href`).

Guests scan the QR code on the main page → land on `upload.html` → tap
"Upload Photos" → send files straight into your Drive folder, no account
needed on their end. You (or Farah) just open that Drive folder anytime to
view or download everything.

The QR code itself needs no editing — it's generated automatically from
whatever URL the site is running on, so it'll work correctly once published.

## File structure
```
index.html        (the main site)
upload.html        (guest photo upload — add your Drive link)
assets/cover.jpg   (ready)
assets/music.mp4   (add once you send the song)
```
