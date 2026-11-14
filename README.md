# arvindmaiya.github.io

Pocket Door's site moved to https://pocketdoor.github.io (repo `pocketdoor/pocketdoor.github.io`) on 14 Nov 2026.
What's left here must stay:
- `pocketdoor/` and `pocketdoor/link/`: redirects to the new site. PC apps from before the move put
  `arvindmaiya.github.io/pocketdoor/link#…` in their pairing codes; the link page hands the code (after `#`) on.
- `.well-known/assetlinks.json`: lets Android open those old codes in Pocket Door (`com.pocketdoor`). Keep it in step
  with the copy on the new site; it lists the fingerprint of every key the app is signed with.
- `.nojekyll`: so GitHub Pages serves the `.well-known` folder.
