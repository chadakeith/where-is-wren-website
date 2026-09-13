# Screenshots

Drop PNGs here with these exact names and they appear on the site automatically.
Until a file exists its slot shows "Screenshot coming soon".

| File | Shows |
|---|---|
| `01-postcard.png` | Play screen at the start of a round: Wren, the first postcard, the globe |
| `02-guess.png` | After a miss: distance, arrow, heat color, second postcard |
| `03-found.png` | Result screen after finding Wren: score, share grid, family scoreboard |
| `04-passport.png` | Passport: country stamps by continent and badges |
| `05-flock.png` | The Flock leaderboard |

## Capturing

In Xcode, run the app on an **iPhone 16 Pro Max** simulator (that size also works
for the App Store's 6.9" slot). Get each screen into place, then either press
`⌘S` in Simulator (saves to the Desktop) or run from Terminal:

```sh
xcrun simctl io booted screenshot ~/Desktop/01-postcard.png
```

Portrait, no status-bar edits needed. Rename to the names above, copy into this
folder, commit and push. The site shows them at about 9:19.5, so any modern iPhone
size crops cleanly.
