NewsMania — Modern News Dashboard
A single-page, responsive news dashboard built with Alpine.js and Tailwind CSS that aggregates news, supports search and filters, and includes lightweight user accounts, article verification, sharing, and a gamified points system.

Quick start
Open finalnews.html in a modern browser, set a MediaStack API key in the code, and start browsing, verifying, and sharing news.

Features
Real-time news feed from MediaStack with keyword, category, and country filters, plus pagination for smooth browsing.

Lightweight auth: register/login, session persistence, and local profile (username, email, avatar).

Gamification: earn points for verifying articles and sharing links; unlock rewards at 50 points.

Article actions: mark verified, share to social platforms or copy link, and track verified/shared counts.

Personalized touches: “You often read about” quick context and basic per-user activity tracking.

Responsive neubrutalism UI with bold borders, shadows, toasts, and modals using Tailwind and Bootstrap Icons.

Graceful empty/error states like “Loading news...” and “No news articles found” with guidance.

Tech stack
HTML5 single-file app with Alpine.js for state and interactivity.

Tailwind CSS utility classes; Space Grotesk font; Bootstrap Icons via CDN.

MediaStack News API for data; LocalStorage/SessionStorage for auth/session and user stats.

Project structure
finalnews.html — all HTML, CSS (inline styles), and JavaScript logic in one file.

Setup
Clone and open

Clone the repository and open finalnews.html directly in a browser, or serve locally.

Recommended local server

Use any static server to avoid CORS or mixed-content issues:

Python: python -m http.server 8000 and visit /finalnews.html.

Configure API key

In the script where MediaStack is called, set access_key to a valid key. Look for the URL template and replace YOUR_API_KEY.

Environment notes

The file loads Alpine.js, Tailwind, Google Fonts, and Bootstrap Icons from CDNs; ensure connectivity.

Usage
Register and login: create an account with username, email, and password; session persists until logout.

Browse: search by keywords, filter by category/country, and paginate through results.

Verify and share: mark an article as verified to earn points; share to social platforms or copy link for extra points.

Rewards: collect points; reach 50+ to claim the reward state indicated in the UI.

Profiles: view username, email, verified/shared counts, and points in the dashboard.

Key UI elements
Dashboard cards showing Verified, Shared, and Points; reward prompt appears at 50+.

“You often read about” panel surfacing common topics from recent activity.

Article cards with source, status badges, and action buttons (Verify, Share, Open).

Toast notifications on actions; modal dialogs for auth and profile where applicable.

Empty/search states: Loading spinner, “No news articles found,” and hints to adjust filters.

Configuration
News API: tweak query params for countries, categories, sort, and page size where the fetch URL is constructed.

Pagination: default grid shows a fixed number of cards per page; adjust page size in code.

Points: update award values for verify/share in the constants where points are incremented.

Styling: adjust neubrutal styles, borders, and shadows via inline CSS and Tailwind utility classes.

Limitations
Client-only app; credentials and points are stored locally, suitable for demos and prototypes.

Relies on public CDNs and MediaStack; rate limits or outages affect functionality.

Roadmap ideas
Move auth, points, and verification to a backend with a database.

Add bookmarking, “read later,” and richer topic modeling for recommendations.

Dark mode and accessibility enhancements for keyboard and screen reader flows.

Contributing
Fork, create a feature branch, commit changes, open a PR. Keep UI consistent with the neubrutal style and add comments near API and points logic.

License
MIT recommended; include a LICENSE file in the repository.

Acknowledgements
MediaStack API for news data.

Alpine.js, Tailwind CSS, Bootstrap Icons, and Google Fonts.
