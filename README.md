# arvindmaiya.github.io

- `pocketdoor/`: Pocket Door's home page.
- `pocketdoor/link/`: where the code on Pocket Door's PC app points. With Pocket Door on the phone, Android opens the
  app straight from the code and this page never shows; without it, the page sends the phone on to get it. The code's
  fields come after `#`, so they never reach this site. The address is permanent: every Pocket Door PC app puts it in
  its codes.
- `.well-known/assetlinks.json`: tells Android that Pocket Door (`com.pocketdoor`) may open those links. It lists the
  fingerprint of every key the app is signed with. Today: this PC's debug key only. Add the Pocket Door
  upload key once it exists, and Google Play's signing key once the app is in Play Console (Play Console › Test and
  release › App integrity shows it).
- `.nojekyll`: so GitHub Pages serves the `.well-known` folder.
