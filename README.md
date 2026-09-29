# Nila 🌙

A little moon who keeps you company. One HTML page, no build step, no frameworks.

## What's in here

| File | What it is |
| --- | --- |
| `index.html` | Nila herself: the moon, costumes, sounds, weather, breathing, journal and memory |
| `manifest.webmanifest` | Tells the iPhone her name, icon and to open full screen |
| `apple-touch-icon.png`, `icon-192.png`, `icon-512.png`, `icon-maskable-512.png` | Home Screen and browser icons |

## 1. Put Nila on GitHub

1. Go to https://github.com/new and create a repository called `nila`. Public or private both work.
2. On the new repository page, click **uploading an existing file**.
3. Select all the files (there are no folders) and upload them together.
4. Click **Commit changes**.

## 2. Create a free Cloudflare account and deploy

1. Sign up at https://dash.cloudflare.com/sign-up and verify your email.
2. In the dashboard, open **Workers & Pages**, then **Create**, then the **Pages** tab, then **Connect to Git**.
3. Connect your GitHub account and choose the `nila` repository. You can give Cloudflare access to only this one repository.
4. On the build settings screen:
   - **Framework preset:** None
   - **Build command:** leave empty
   - **Build output directory:** leave empty (or `/`)
5. Click **Save and Deploy**. After about a minute Nila is live at an address like `https://nila.pages.dev` (or `nila-xyz.pages.dev` if the name is taken).

Cloudflare's screens change from time to time. If a button has moved, look for "Pages" and "Connect to Git".

From now on, every change you commit to GitHub goes live by itself within a minute.

## 3. Add her to your iPhone Home Screen

1. Open the `pages.dev` address in **Safari** (not Chrome, not the Claude app).
2. Tap the **Share** button, then **Add to Home Screen**, then **Add**.
3. Open Nila from her new icon. She opens full screen, like an app.

## 4. Bring your memories and journal along

Memories and journal entries you made while using Nila inside claude.ai are saved to your claude.ai account, which the hosted Nila can't reach. To move them:

1. Open Nila in claude.ai, tap the **⋯** button, then **Export a backup**. Save the file to the Files app.
2. Open the hosted Nila, tap **⋯**, then **Import a backup**, and choose that file.

Importing never deletes anything; it merges.

## Good to know

- **Weather:** the hosted Nila shows live Madurai weather from Open-Meteo (free, no key needed).
- **Your data:** memories and journal are saved in Safari's storage on your phone. Export a backup now and then. The Home Screen app and Safari tabs keep separate storage, so use Nila from one place.
- **Sounds:** tap her once after opening so iOS allows sound.
- **Her brain:** replies are still built-in lines. Connecting her to Claude comes next, using a small Cloudflare Worker to keep the API key secret.
