# Gender Reveal Digital Invitation

A responsive, mobile-friendly digital version of the supplied invitation. The RSVP area over the orange button and the backup RSVP button both open the supplied Google Form.

## Files

- `index.html` — invitation webpage, clickable RSVP overlay, backup RSVP button, and social preview metadata
- `invite.png` — original invitation artwork
- `.nojekyll` — tells GitHub Pages not to run Jekyll processing

## Publish with GitHub Pages

1. Unzip this folder.
2. Create a new GitHub repository. A suggested name is `gender-reveal-invite`.
3. Upload **the contents of this folder** (not an extra enclosing folder) to the repository's root:
   - `index.html`
   - `invite.png`
   - `.nojekyll`
4. In the repository, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**, select the `main` branch and `/ (root)`, then Save.
6. Wait for GitHub Pages to publish. Your site address will look like:
   `https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/`

## Important: enable accurate text-message link previews

Before sharing the link with guests, edit `index.html` and replace **every** occurrence of:

- `YOUR-USERNAME` with your GitHub username
- `YOUR-REPOSITORY` with your repository name

These placeholders appear in the canonical URL and social preview metadata (`og:url`, `og:image`, and Twitter image fields). The `og:image` must point to the publicly accessible `invite.png` on your live GitHub Pages site. Commit the changes and allow the site to republish.

Then text the published website URL (not the Google Form URL) to yourself as a test. Preview behavior varies by messaging app, device settings, and cached link data; some apps may not show a preview immediately. The website cannot force a preview or send texts to guests.

## RSVP button placement

The transparent tap target is positioned over the orange RSVP button in the supplied artwork. It scales with the image on phones and tablets. The separate RSVP NOW button below the artwork provides an accessible fallback.

If you change the artwork or crop it, the overlay coordinates may need to be adjusted in the `.image-rsvp` CSS rule.

## Compatibility

Uses standard HTML and CSS, a responsive viewport, and ordinary HTTPS links. It is designed for current iOS Safari, Android Chrome, and desktop browsers. The RSVP form opens in a new tab/window.
