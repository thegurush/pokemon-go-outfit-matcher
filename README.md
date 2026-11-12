# Pokémon GO Outfit Matcher (static prototype)

A free, no-API-key GitHub Pages prototype using the wardrobe screenshots extracted from the user's Universal Wardrobe Reference v7. No Pokémon image is uploaded to a server; all sampling happens in the browser. Saved outfits are stored in browser localStorage; export JSON to back them up.

## Deploy

1. Create a new GitHub repository (e.g. `pokemon-go-outfit-matcher`).
2. Upload **all** files in this folder, preserving the `assets/` folder and `pages.json`.
3. Go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, branch **main**, folder **/(root)**, and Save.
4. Open the GitHub Pages URL after deployment finishes.

## What works
- Pokémon photo upload and click-to-sample color palette, with editable roles.
- Browse all wardrobe screenshot pages 2–34, with category and page navigation.
- Tap wardrobe screenshots to add candidates, confirm row and column, and add notes.
- Build an outfit shortlist, save locally, load/delete saved outfits, export JSON.
- Universal color-matching rules are displayed on-page.

## Limitations / next phase
- This is a **manual visual matching tool**, not an AI-powered outfit recommender. It does not automatically detect individual garments, score their visible colors, or generate a complete recommended outfit. Implementing trustworthy automatic ranking requires individually segmented item images and a structured inventory; screenshot backgrounds and swatch variations make naive pixel matching misleading.
- Item crop previews use an approximate image focus, not accurate segmentation. The full screenshot is the authoritative reference.
- User-selected row is confirmed manually; screenshot row spacing varies.
- A new phone/browser will not automatically share saved outfits; use exported JSON as backup (import is not yet implemented).
- The app has no affiliation with Niantic or The Pokémon Company. All wardrobe images are user-provided reference screenshots.
