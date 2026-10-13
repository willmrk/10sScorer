# 10sScorer# 10s Score Keeper

A simple, mobile-friendly score keeper for the card game Tens. Play with physical cards and use this web app to record scores on an iPhone, Android phone, tablet, or computer.

## Features

- Enter player names before starting a game.
- Record each player's points after every round.
- Play as many rounds as you choose.
- View round-by-round scores and running totals.
- Highlight the player with the lowest total, including ties.
- Edit previous rounds to correct mistakes.
- Save the current game automatically in the browser.
- Download scores as a CSV file.

## Scoring

The objective of Tens is to have the **lowest total score**.

- Scores must be whole numbers of **zero or more**.
- **At least one player must score zero in every round.**
- More than one player may score zero.
- Every player needs an entered score before a round can be saved.
- Corrections to earlier rounds update the running totals.

## How to use

1. Open the app in your browser.
2. Enter at least two player names. Use distinct names to identify each player.
3. Select **Start game**.
4. After playing a round with your cards, enter each player's score, including any zeros.
5. Select **Save round** to update the totals and round history.
6. Continue adding rounds until your group decides to stop.

Use **Edit** beside a round to change its scores. Use **Download scores** to keep a copy. **New game** clears the current game after confirmation, so download the scores first if you want to preserve them.

## Run locally

Open `10s-score-keeper.html` in a web browser. No installation, account, dependencies, or build step is required.

## Host on GitHub Pages

GitHub Pages can host this app as a static website. It is available with GitHub Free for public repositories.

### Use a separate repository

1. Create a public GitHub repository, for example `10s-score-keeper`.
2. Upload `10s-score-keeper.html` to the repository root, renaming it **`index.html`**.
3. Optionally upload this README as `README.md`.
4. Open the repository's **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Choose the branch containing your files, typically **main**, and the **/ (root)** folder. Select **Save**.
7. Wait for publication, then open the website address shown in the Pages settings.

The usual address is:

```text
https://YOUR-USERNAME.github.io/10s-score-keeper/
```

Replace `YOUR-USERNAME` with your GitHub username. Publication can take up to ten minutes.

### Add it to an existing GitHub Pages site

If you already have a site at `https://YOUR-USERNAME.github.io/`, place the app in a `10s` folder inside the site's publishing source and name it `index.html`:

```text
10s/
  index.html
```

After publication, open:

```text
https://YOUR-USERNAME.github.io/10s/
```

Use the publishing source selected in **Settings → Pages**. For example, if the site publishes from `/docs`, put the app at `docs/10s/index.html`. If the existing site uses a custom build workflow, ensure that workflow includes the app in its published output.

### Update the app

Replace the published `index.html` with the updated app file and commit the change. GitHub Pages will publish the update using the site's configured deployment process.

Official instructions: [Creating a GitHub Pages site](https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site) and [GitHub Pages quickstart](https://docs.github.com/en/pages/quickstart).

## Score storage and privacy

Scores are stored in **local storage in the browser on the device being used**. The app does not send player names or scores to a server and does not synchronize games between devices or browsers.

- Use the same browser on the same device to resume a saved game.
- Clearing browser data can remove the saved game.
- Private browsing may not retain scores after the session closes.
- Moving from the local file to a hosted website does not transfer the saved game automatically.
- Download a CSV copy before clearing scores or browser data.

Hosting makes the app available from a web address. The current version does not include a service worker, so opening the hosted app without an internet connection is not guaranteed.

## Technology

The application is one self-contained HTML file with embedded CSS and JavaScript. It uses browser local storage for saving scores and requires no backend or database.
