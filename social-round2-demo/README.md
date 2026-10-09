# Loop — Social Media Platform, Round 2

An animated Instagram/TikTok-inspired social media frontend demo. It is in a separate folder from the learning-platform demo and includes only the requested Round 2 functionality.

## Run locally

```sh
python3 -m http.server 4174 --bind 127.0.0.1 --directory dist
```

Open http://127.0.0.1:4174.

## Features

- Create a text post (1–500 characters), stored in this browser and displayed at the top of the feed.
- View a chronological feed with sample photo and text posts.
- Like a post with an animated heart, or double-tap its media. One like per demo user per post; repeated likes do not increase the count.
- Add comments (1–300 characters).
- See simulated notification delivery to the author after successful likes/comments.
- Delete your own posts, with a preview confirmation. Other authors’ posts cannot be deleted.
- Review the five REST API designs, methods/URIs, Create Post request and response, status codes, sequence, and actual simulated request log in **Round 2 API design**.

## Scope and limitations

This is a static frontend demo, not an HTTP API server. A central JavaScript function simulates all five APIs. Fixed current user: `usr_alex`. Browser localStorage saves demo posts, comments, likes, and notification records on this device. No cross-device synchronization, real login, real push notifications, media uploads, messages, follows, search, sharing, video playback, or Round 3 infrastructure is included.

Notifications are a delivery simulation showing both the actor and recipient; this is not the current user’s personal inbox. The sample engagement counts are fictional demo data. New posts start with zero engagement.

Animations include gradient motion, gentle photo motion, feed entry, modal entry, heart bursts, like-button bounce, notification entry, and post removal. The layout supports desktop and mobile and honors reduced-motion settings.

Clear this site’s browser storage to reset the sample data.

## Files

- `dist/index.html` — page structure
- `dist/styles.css` — styling, animations, responsive layout
- `dist/app.js` — sample content, central API simulation, state, interactions, API documentation
- `dist/assets/coastal-moment.png` — original sample-post photograph, 1122 × 1402, generated with the built-in image_gen tool

## Original image prompt

Use case: photorealistic-natural. Portrait 4:5 editorial lifestyle photograph of a fictional adult skateboarder in mid-motion on a sunny coastal promenade beside a turquoise sea. Saturated warm pink/orange sunset and blue shadows; relaxed indie-magazine aesthetic, subtle film grain, dynamic diagonal composition, full skateboard visible, a little negative space at the top. No text, logos, watermark, UI, or screenshot elements.
