# Fact or Hasbara?

Y+ (yplus.ps) media-literacy experience, story 2 of the Communicating Palestine toolkit.

- `index.html`: the interactive (also as `Fact or Hasbara.dc.html`)
- `fact-or-hasbara-data.json`: all content in EN / IT / FR / AR: items, sources, stories, advocacy, messageBank
- `support.js`: runtime
- `assets/yplus-logo.png`

Serve over HTTP (GitHub Pages works); the page fetches the JSON.

## URL parameters
`?lang=ar|en|it|fr`, `?deck=daily`, `?mode=kiosk`

## Editing content
Add a question by adding an object to `items` in the JSON. Set `status: "published"`, a future `reviewBy`, and all four `translationComplete` flags, or it will not enter a deck. Set `messageBank.goDeeperUrl` and `messageBank.actionUrl` to show those buttons.

GA4 Measurement ID G-NMEYZ7ZWB5 is built in; events use the `foh_` prefix.
