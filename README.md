# Nursery Activity Journal

A home-screen app for one nursery teacher on one iPad: log each day's activities and how
the children responded, plan the week, and get suggestions for what to try next.

It is a web app that installs to the iPad Home Screen. It opens full screen with its own
icon and works without internet. Nothing is installed from the App Store.

## Files

| File | What it is |
| --- | --- |
| `index.html` | The whole app |
| `manifest.webmanifest` | Name, colours and icons for the Home Screen |
| `sw.js` | Keeps the app working offline |
| `icon-180.png`, `icon-192.png`, `icon-512.png` | App icons |

All six files must sit together in the same folder.

## What it does

- **Today**: log an activity in about a minute. Tap stars for involvement and a face for
  wellbeing (the five-point Leuven scales), tick what you noticed, add a note and a next step.
- **Week plan**: a colour-coded row for each day, Monday to Friday. Move activities between
  days, tick off a "Get ready" checklist of materials and prep, and see which areas of
  learning the week covers.
- **Ideas**: coloured flashcards drawn from the log (what absorbed the children, what fell
  flat, which areas are thin). The front shows the reason, materials, prep time, activity
  time and group size; flip the card for the steps. Plus an idea board for your own ideas.
  Prep times on the starter activities are estimates.
- **Activity library**: 17 starter activities as flip cards. The front shows materials,
  prep time, group size and ages; the back shows the steps and the research. Each is tied
  to a published source and labelled with the kind of evidence behind it. Add your own.
- **Patterns**: flip-card insights (most absorbing activity, least covered area, and what
  to do about each), plus coverage by area of learning and involvement by kind of play.

## Step 1: give it a web address (once)

The iPad needs a web address to install from. GitHub Pages is free:

1. Create a GitHub account at https://github.com and sign in.
2. Create a new **public** repository, for example `nursery-journal`.
3. Upload all six files with **Add file > Upload files**, then commit.
4. Open **Settings > Pages**. Under **Build and deployment**, choose
   **Deploy from a branch**, branch `main`, folder `/ (root)`, and save.
5. After a minute or two the app is live at
   `https://YOUR-USERNAME.github.io/nursery-journal/`.

## Step 2: install it on the iPad (once)

1. Open that address in **Safari** on the iPad.
2. Tap the **Share** button, then **Add to Home Screen**, then **Add**.
3. Open the app from its new icon and clear the example entries.

Install first, then start logging. The Home Screen app keeps its own entries, separate
from anything typed in Safari.

## Privacy and backups

- The web address is public, but entries are **not** uploaded anywhere. They are saved
  on the iPad.
- Use initials or group names, never children's full names.
- Entries do not sync to other devices. **Back up or restore > Save a backup file**
  saves a file to the Files app, and the same screen restores it on another device.
- Removing the app from the Home Screen can delete its entries. Save a backup first.

## Updating the app

Upload the changed files to the repository. If `index.html` changed, also raise the
version in the `CACHE` line at the top of `sw.js` (for example `v4` to `v5`). The app
picks up the new version the next time it is opened with internet.

## Artwork

The icons, faces, mascot and app icon were drawn for this app. To use your own artwork,
replace the three icon PNG files, or send SVG files to swap into `index.html`.

## Sources behind the starter activities

- Department for Education, Early years foundation stage statutory framework (2025).
- Education Endowment Foundation, Early Years Toolkit.
- Laevers, F., Leuven scales for wellbeing and involvement.
- Center on the Developing Child at Harvard University (2014), Enhancing and Practicing
  Executive Function Skills with Children from Infancy to Adolescence; 5 Steps for
  Brain-Building Serve and Return.
- Whitehurst et al. (1988), Developmental Psychology (dialogic reading).
- Verdine et al. (2014), Child Development (block building and early maths).
- Ramani and Siegler (2008), Child Development, 79(2), 375-394 (number board games).
- Bryant, Bradley, Maclean and Crossland (1989), Journal of Child Language, 16(2), 407-428.
- Nicolopoulou et al. (2015), Early Childhood Research Quarterly, 31, 147-162.
- Grissmer et al. (2010), Developmental Psychology, 46(5), 1008-1017.
- Fjortoft (2004), Children, Youth and Environments, 14(2), 21-44.
- Williams et al. (2015), Early Childhood Research Quarterly, 31, 113-124.
- Domitrovich, Cortes and Greenberg (2007), Journal of Primary Prevention, 28, 67-91.
- Nicholson (1971), How NOT to Cheat Children: The Theory of Loose Parts.
- Goldschmied and Jackson (1994), People Under Three.

Links to each source are on the activity cards in the library.
