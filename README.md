# Shanvik MK – Little Maharaja Digital Invitation

Static website for Vercel.

## Publish through GitHub + Vercel
1. Create a new **private** GitHub repository, e.g. `shanvik-mk-invitation`.
2. Upload `index.html`, `vercel.json`, `og-shanvik.png`, and the entire `assets/` folder to the root of that repository (not the ZIP itself).
3. Vercel → Add New → Project → Import Git Repository → select this repository.
4. Framework Preset: **Other**; Build Command: **none**; Output Directory: project root. Deploy.
5. In `index.html`, replace ALL `https://shanvik-mk-invitation.vercel.app/og-shanvik.png` with the actual deployed domain followed by `/og-shanvik.png`; commit/push to redeploy. The OG preview only works with the public HTTPS image URL.
6. Validate sharing with Facebook Sharing Debugger, WhatsApp, and LinkedIn Post Inspector; previews are cached.

The original user-supplied 4:3 poster is copied byte-for-byte into `og-shanvik.png`. WhatsApp cannot be forced to hide its text URL while keeping a clickable destination: the app controls this. Sharing the image as media displays just the image, without a clickable site link.

RSVP/Wishes in this frontend are preview-only and require a backend to store online submissions.
