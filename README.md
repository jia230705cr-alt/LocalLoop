# Cloud & Stories · LocalLoop

A bilingual Bristol discovery prototype for an innovation course. Existing Cloudy branding is retained, with working discovery, route links and an explicitly simulated booking journey.

## Preview

Run `python3 -m http.server 4173 --bind 127.0.0.1` in this directory and open http://127.0.0.1:4173/.

No build or package installation is needed. GitHub Pages serves these files directly.

## Files

- `index.html`: accessible shell and native dialog.
- `styles.css`: responsive layout, typography, contrast and reduced-motion support.
- `data.js`: bilingual **illustrative** experiences, proposed prices, route stops and sample stories.
- `app.js`: search, combined date/category/budget filters, 28-day sample schedule, details, demo booking, local plans, route links and private notes.
- `cloudy.svg`: mascot preserved from the original site.

## Prototype boundaries

Activity prices, dates, hosts, inclusions and meeting points are planning examples, not contracted inventory. No payments, real bookings, authentication, emails, public posting or live chat are implemented. Demo plans, language, saved stories and private notes use browser localStorage and are not sent to a server. Clearing browser data removes them. Private notes are escaped before display.

Walking routes link to Google Maps with named start/end points and a waypoint. Distances and durations are approximate planning estimates, not live navigation results. External map providers determine actual access, paths and travel times. Photos are illustrative, loaded from Unsplash; typefaces load from Google Fonts, with system-font fallbacks.

## Verification (2026-11-09)

- JavaScript syntax: `node --check app.js` and `node --check data.js`.
- Browser: keyword search, empty results, combined category/budget filtering, reset.
- Booking: details, date/time choices, 3-person total (£18 × 3 = £54), acknowledgement, save, reload persistence and removal.
- Chinese-language search and translated interface.
- Route selection updates Google Maps start/end/waypoint URL.
- Mobile menu opens and closes on selection; 390px layout has no horizontal overflow.
- Desktop visual review and browser console check.

Before a real launch, confirm suppliers, dates and prices; implement backend authentication, inventory and transaction handling; research cancellation/access requirements with partners; and run usability tests with target users.
