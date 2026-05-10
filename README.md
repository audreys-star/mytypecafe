# MyTypeCafe

MyTypeCafe is a cozy browser-based typing practice app with custom text, file upload support, local progress saving, stats, levels, and a daily XP goal.

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

1. Create a public GitHub repository named `mytypecafe`.
2. Push this project to the repository.
3. In GitHub, open **Settings -> Pages**.
4. Set the source to **GitHub Actions**.
5. The included workflow will publish the site automatically.

## Notes

The current Gmail button is a demo login that stores progress in the browser with `localStorage`. Real Google sign-in would need an auth provider such as Firebase Auth or Supabase Auth.
