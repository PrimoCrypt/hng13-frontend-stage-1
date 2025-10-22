# Profile Card (HNG Stage 0)

A simple static profile card built with plain HTML and CSS. This small project displays a user avatar, bio, current timestamp (updates every second), social links, hobbies, and dislikes. It includes data-testid attributes useful for automated testing.

## What you get

- `index.html` — The profile card markup and a tiny inline script that updates the current time (in milliseconds).
- `style.css` — Styles for the profile card.
- `images/` — Contains the avatar image `slackDisplayPicture(250px by 250px).png` used by the card.

## File structure

```
hng13-frontend-stage-0/
├─ index.html
├─ style.css
├─ README.md
└─ images/
	 └─ slackDisplayPicture(250px by 250px).png
```

## How to preview

You can open `index.html` directly in your browser (double-click or use the browser's file > open).

## Notes about the implementation

- The current time is shown in milliseconds and is updated every second by a small inline script in `index.html`:

  - The element with id `user-time` is populated via `Date.now()` and refreshed with `setInterval`.

- The markup uses `data-testid` attributes that are useful for test runners and automated checks. Key test ids:

  - `data-testid="test-profile-card"` — the article wrapper for the card
  - `data-testid="test-user-avatar"` — the avatar `<img>`
  - `data-testid="test-user-name"` — the user name `<h2>`
  - `data-testid="test-user-bio"` — the bio paragraph
  - `data-testid="test-user-time"` — the timestamp element
  - `data-testid="test-user-social-twitter"` and `test-user-social-github` — social links
  - `data-testid="test-user-hobbies"` and `test-user-dislikes` — lists
