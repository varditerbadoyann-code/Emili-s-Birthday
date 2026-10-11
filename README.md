# Emili's Birthday

A one-page invitation website for Emili's 7th birthday spa party at Pink SPA in Bratislava, on Saturday, 17 October 2026, from 15:30 to 18:00.

Guests open the link from a WhatsApp message, so the page is designed for phones first. It also works on larger screens.

## What's on the page

| Section | What it does |
|---|---|
| **Hero** | "Emili is turning 7", the date, time and place, and a button to the party details |
| **A letter from Emili** | A short invitation in Emili's own words, written to be read aloud to a 7-year-old |
| **The party details** | A countdown in "sleeps", date, time (15:30 – 18:00), place, what to wear, and an Add to Google Calendar link |
| **What we'll do** | The 2.5-hour party plan: welcome, pamper time, glow-up, neon fashion show, disco, birthday wishes, pick-up |
| **How to find us** | A simple illustrated map, the address with a copy button, free parking in front of the building, and links to Google Maps, Apple Maps and Waze |
| **While the girls are at the spa** | For moms: coffee at the Cinnabon café in Nivy shopping center during the party, with a link to the menu |
| **Will you come?** | How to reply by 12 October: a WhatsApp message or a text |
| **Footer** | A thank-you from Emili |

## How it's built

- One static HTML file (`index.html`) with inline CSS and a little plain JavaScript. There's no build step and there are no dependencies.
- Fonts come from Google Fonts: Pinyon Script, Young Serif and Nunito Sans.
- Phones get their own layout below 760 px wide. `<picture>` elements make sure each device downloads only the image it shows.
- The countdown is calculated in Bratislava time, so guests in other time zones see the same number.
- Copy buttons announce their result to screen readers, and animation respects reduced-motion settings.

## Files

```
index.html               the whole page
img/                     illustrations (JPEG, plus PNG where transparency is needed)
menu/cinnabon-menu.pdf   café menu without prices, opened by "See the menu"
```

## View it locally

Open `index.html` in a browser. No server is needed.

## Publish with GitHub Pages

In the repository settings, go to **Pages**, choose **Deploy from a branch**, pick `main` and the `/ (root)` folder, and save. The site is then served at `https://<username>.github.io/Emili-s-Birthday/`.

## Credits

- The illustrations of Emili, her friends and the café scene were created for this invitation. The other girls and moms are fictional characters, not real people.
- The party package and the venue belong to [Pink SPA](https://www.pinkspa.sk/).
- The menu PDF was assembled from Cinnabon Slovakia's menu images for guests' convenience. Cinnabon is a trademark of its owner, and items may vary in the café.
