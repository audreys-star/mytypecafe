# Audrey's TypeCafe

Audrey's TypeCafe is a cozy browser-based typing practice app with custom text, file upload support, local progress saving, stats, levels, and a daily XP goal.

## Features

- Word-by-word typing practice
- WPM, accuracy, errors, streak, XP, and level tracking
- Paste custom text or upload `.txt`, `.md`, `.html`, and `.pdf` files
- Demo profile with browser-local progress saving
- Focus mode, sound toggle, readable font mode, and high contrast mode
- Installable PWA metadata with a service worker and app icon

## Project Structure

```text
.
├── index.html
├── manifest.json
├── sw.js
└── icons/
    └── icon.svg
```

## Local Preview

Because this is a static website, you can open `index.html` directly in a browser.

For a local server preview:

```bash
python3 -m http.server 4173
```

Then visit:

```text
http://localhost:4173
```

## Deploying To GitHub Pages

1. Push this project to the GitHub repository.
2. In GitHub, open **Settings -> Pages**.
3. Set the source to **Deploy from a branch**.
4. Choose branch `main` and folder `/ (root)`.
5. Save and wait for GitHub Pages to publish the site.

## Custom Domain

The desired custom domain is `audreystypecafe.com`.

Only add the `CNAME` file after the domain is purchased and its DNS points to GitHub Pages. Until then, use the GitHub Pages URL so the site stays reachable.

## Notes

The current Gmail button is a demo login that stores progress in the browser with `localStorage`. Real Google sign-in would need an auth provider such as Firebase Auth or Supabase Auth.
