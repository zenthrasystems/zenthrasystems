# Publish your cinematic README on a personal GitHub profile

This package is configured for an **individual/personal GitHub account**, with Zenthra Systems as the public-facing brand. It is **not** an organization `.github/profile/README.md` package.

## The required setup

1. Sign in to GitHub and confirm your exact **username** (the handle in `github.com/YOUR_USERNAME`). Your display name does not count.
2. Create a **public** repository whose name is **exactly your GitHub username**. In your case: create `zenthrasystems/zenthrasystems` (or rename the current `zenthrasystems-` repository).
3. Place the **top-level `README.md`** from this package in the repository's **root**, not inside a `profile/` or `.github/` subdirectory.
4. Upload the entire **`assets/`** folder next to `README.md`, retaining names and directory structure.
5. Commit to the repository's default branch, then visit `https://github.com/zenthrasystems` to see the profile README.

```
zenthrasystems/       ← repository named exactly like your username
├── README.md         ← shows on personal profile
└── assets/
    ├── hero-motion.gif
    ├── hero-poster.jpg
    ├── integration-motion.gif
    ├── integration-poster.png
    ├── logo-dark.png            ← theme-aware horizontal logo (dark mode)
    ├── logo-light.png           ← theme-aware horizontal logo (light mode)
    ├── logo-mark.png            ← standalone brandmark (ideal for GitHub avatar)
    ├── Zenthra_Systems_logo_2.png
    ├── Zenthra_Systems_logo_6.png
    ├── Zenthra_Systems_logo_7.png
    ├── service-1.png ... service-4.png
    ├── showcase-1.png ... showcase-3.png
    └── contact-banner.png
```

You can keep the brand-oriented design on a personal profile. The introduction uses a collaborative team voice ("We/our"); replace it with your preferred name and professional title if you want them shown publicly.

## Additional personal-profile improvements (optional)

- **Avatar:** Use `assets/logo-mark.png` (or `assets/Zenthra_Systems_logo_2.png`) as your GitHub account profile picture for unified corporate branding.
- Add a recognizable profile **bio** to your GitHub account (e.g. *"Welcome to Zenthra Systems, a premier IT company where human ingenuity meets Artificial Intelligence."*).
- Pin your best public repositories and provide actual demo links where available.
- Check the displayed profile in **dark/light modes** and on mobile. GIF support is subject to clients and accessibility settings.
- If your public handle differs from `zenthra-systems`, update any account-specific profile links or services you add later.
- Verify every public project metric, location, contact address, and capability claim before publication.

## Technical notes

- All graphics are self-hosted in `assets/` with relative paths from the README; **do not upload only the Markdown file**.
- Hero and integration graphics use GIF motion with static poster fallbacks in `<picture>` tags for `prefers-reduced-motion` in supported renderers. GitHub restricts arbitrary HTML/CSS/JS, so avoid trying to insert animated JavaScript.
- If you prefer no motion or want faster download times, replace `hero-motion.gif` and `integration-motion.gif` in `README.md` with the included static files.
- Dashboard graphics are illustrations, not actual live software screenshots. The revenue/conversion figures in the mobility example are supplied by your original README and not independently verified; modeled results are labeled appropriately.
- The discovery call action is a **mail link**, not an actual scheduling-booking service.

## Verified GitHub references

- Personal profile README: https://docs.github.com/en/account-and-profile/how-tos/profile-customization/managing-your-profile-readme
- Personal profiles and GIFs: https://docs.github.com/en/account-and-profile/concepts/personal-profile
- Repository-relative images and Markdown formatting: https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax
