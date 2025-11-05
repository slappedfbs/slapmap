# SlapMap

A hyper-specific guide to the East Bay rendered with Leaflet, CSV data, and lo-fi UI flourishes.

## Google My Maps Upsell

Use the new **Get the Map** page (`get-the-map.html`) to sell access to a private Google My Maps copy
of SlapMap:

1. Create or duplicate a My Maps project under an account you control and set sharing to "Anyone with
the link".
2. Generate a hosted checkout URL (Stripe Payment Link, Gumroad, etc.) and configure its success
redirect to `https://<your-domain>/get-the-map.html?success=1`.
3. Edit `get-the-map.html` and swap the placeholder checkout URL and Google Map link with your real
links.
4. Optional: share `get-the-map.html?preview=1` with friends or testers to bypass the purchase flow.

Visitors who complete checkout are redirected back to the page where the private link is revealed. If
an old link leaks, create a fresh My Maps duplicate and update the href in the file.

## Development

Everything is static, so open `index.html` in a browser or host the folder with any static server.
Leaflet pulls data from the bundled CSV file. 
