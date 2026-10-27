# Singapore Property News

Static site for automated property news summaries aimed at Singapore home buyers and sellers.

## Deploy to Netlify

1. Go to [Netlify](https://app.netlify.com)
2. Add new site → Import an existing project
3. Connect GitHub and select `sellingsgproperty-ctrl/sg-property-news`
4. Build settings: leave blank (static HTML, publish directory = root)
5. Deploy

You can then set a custom domain or use the `.netlify.app` URL, and link it from your main site as a /news subpage or subdomain.

## Updates

An automation checks the PropNex Telegram channel hourly during Singapore daytime (08:00–22:00) and generates clean HTML fragments with summaries + buyer/seller insights. 

To publish: append the new fragment into `index.html` inside `<main id="news">` (newest on top), commit, and Netlify will redeploy automatically once connected.
