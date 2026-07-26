# Blog import — LinkedIn archive → building-schools-site (26 July 2026)

Drop-in update for TheNovacene/building-schools-site. Contents:

- `blog/` — 69 new posts in the site's existing template (header, chips, post-body, footer), filenames matching the house bare-slug style. No existing file is overwritten.
- `blog/index.html` — REPLACES the current index: all 92 posts (23 existing + 69 new) merged in reverse-chronological order. Existing cards untouched.
- `blog/images/` — 23 Canva banners renamed `banner-*.png`, wired into their posts.

One manual step: append the rule below to the end of `style.css` (also saved here as `style-addition.css`) so post images scale inside the article column:

    article.post .post-body img { max-width: 100%; height: auto; border-radius: var(--radius); box-shadow: var(--shadow); }

Notes:
- Four banner matches are educated guesses — check these pairs: learning nature → Tech Should Be Invisible; neo maths → When Geometry Teaches Geography; LTIE → Beyond the Census; lego → The Place for Schools in the Cloud. Unmatched banners (not included): 1.png (Newcastle), 5.png (Mnemonic Resonance Simulator), containment (pillars), cry for help (→ the unpublished Void piece), polytunnels (→ Yarn Bombs, not in this set), glyphonics logo.
- 64 in-body images still point at LinkedIn's CDN and expire 6–13 August 2026 — replace with local copies in blog/images/ when rescued.
- Each republished post ends with a "First published … on LinkedIn" link. Posts with co-author flags (IBM/Adam Ring, Natasha McIntosh, Eve¹¹ credit) carry the same text as published — clear consents before pushing those three, or hold them back. The Planning for Dancing in Rain post has been lightly edited to soften the TutorCruncher product focus (noted in its footer); all other posts are untouched.
