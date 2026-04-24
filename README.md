# a little question

A single-page site that asks one question. If she says no, the "Yes" button grows, the "No" text gets sillier, and the No button starts dodging. When she says yes, a card reveals the date and time — place stays a surprise.

## Preview it locally

Just open `index.html` in a browser. That's it — it's fully static.

Or, if you want a local server:

```bash
# Python
py -m http.server 8080
# then open http://localhost:8080
```

## Add your photos (optional but recommended)

Drop 3 square-ish JPGs into `images/`:

- `images/photo-1.jpg`
- `images/photo-2.jpg`
- `images/photo-3.jpg`

If any are missing, the polaroid falls back to a soft gradient — nothing breaks.

## Host it so she can just open a URL

Pick one. All are free.

### Option A — Vercel (recommended, ~60 seconds)

```bash
npm i -g vercel
vercel
```

Answer the prompts (defaults are fine). You get a URL like `your-project.vercel.app`.
Run `vercel --prod` after to promote the production URL.

### Option B — Netlify drop

Go to https://app.netlify.com/drop, drag the whole `Sandy` folder onto the page. Done.

### Option C — GitHub Pages

Push the folder to a public repo, enable Pages in Settings → Pages → deploy from `main` branch root.

## Things you can tweak

All copy is in `index.html`:

- Title: search `Will you go on a date with me`
- Date / time values: search `May 6` and `5:00 PM`
- "No" button's funny responses: search `noTexts`
- Sub-line responses: search `subTexts`
- Signoff: search `can't wait`

Good luck. You've got this.
