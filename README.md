# Maple Ridge Durga Puja 2026

The website for the **19th Year Shri Shri Durga Puja**, hosted by Anita Roy Chowdhury and Family.

- **Dates:** October 16–19, 2026 (Maha Sasthi to Maha Navami)
- **Address:** 21186 Wicklund Ave, Maple Ridge, BC V2X 3R9 (for GPS, use 21188 Wicklund Ave)
- **Phone:** 604-763-4820

It is a single static page (`index.html` plus `assets/idol.jpg`) served by GitHub Pages. There is no build step.

## Editing the schedule

All content lives in `index.html`.

- **Days and times:** each day is an `<article class="day" data-date="YYYY-MM-DD">` block in the `#schedule` section. Change the `data-date`, the weekday and date labels, and the times inside `.times`.
- **Countdown:** in the `<script>` at the bottom, update the two `Date.parse(...)` lines. `start` is when Maha Sasthi begins and `end` is when the "Puja is on now" message switches to the thank-you message. Times use the Pacific offset (`-07:00` during daylight time).
- The schedule highlights today's date (Pacific time) and dims past days automatically.
