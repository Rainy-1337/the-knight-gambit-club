# Knight Gambit Chess Club — Website

## Files
- `index.html` — home page, about section and membership registration form
- `announcements.html` — announcements page (edit the list at the top of the script)
- `style.css` — colours, animations and layout
- `logo.png` — club logo

## Run it
Open `index.html` in a browser. To put it online, upload the whole folder to any static host (GitHub Pages, Netlify, Vercel).

## Get registration emails (Formspree, free)
Browsers cannot send email on their own, so the form uses Formspree to forward each registration to your inbox.

1. Go to https://formspree.io and create a free account with your club email.
2. Click **New Form**, give it a name, and copy the form ID (looks like `xabcdwzy`).
3. Open `index.html`, find this line near the bottom and paste your ID:
   ```js
   const FORM_ENDPOINT = "https://formspree.io/f/YOUR_FORM_ID";
   ```
4. Confirm the activation email Formspree sends you. Each registration will then arrive in your inbox with the full name, CIN and filière.

## Edit announcements
Open `announcements.html`, edit the `announcements` array in the script, and save. Newest items go first.

## Notes
- CIN is validated as 1 or 2 letters followed by 5 to 8 digits. Adjust the pattern in `index.html` if needed.
- Personal data (CIN) is sent by email. Consider keeping the inbox private, and only collect what you need.
