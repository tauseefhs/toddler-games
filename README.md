# Toddler Games

Simple browser games I make for my toddler. Free to use, change and share.

## Why I made this

Most games for small kids are full of ads, push in-app purchases, or cost a lot. And even the good ones aren't made for *your* kid: what they love right now, what they can do, how long they can focus.

So I started making my own. Small, calm games built around what my toddler is into, with no ads, no tracking and nothing to buy. More games will come over time as he grows and his interests change.

If you're a parent who wants the same for your kid, take what's here. Use the games as they are, change them, or use them as a starting point for your own.

## Games

| Game | What you do |
|---|---|
| [Dino Dash](site/games/dino-dash/) | Run with the dino, jump over rocks, eat fruit, hatch baby dinos and ROAR. Tap to jump (or Space on a keyboard). |

## Play them

The games are plain web pages. No install, no account.

- **Quickest:** download this project (green **Code** button, then **Download ZIP**), unzip it and open `site/games/dino-dash/index.html` in a browser.
- **On a phone or tablet:** host the `site` folder anywhere that serves web pages, then open it on the device and hold it sideways. Adding it to the home screen makes it feel like an app.

## How the games are made

These are the rules I follow for every game. They're the part most worth copying.

- **Landscape first**, for a phone or tablet held sideways.
- **Big touch targets.** Small fingers miss.
- **No reading needed.** Pictures, colours and sounds do the explaining.
- **Forgiving.** Mistakes cost a little, never everything. In Dino Dash, baby dinos take a bump for you before you lose a heart.
- **Sound that can be turned off.**
- **Nothing from outside.** No ads, no tracking, no outside requests. Fonts and pictures are stored with the game.

## Add your own game

1. Make a folder under `site/games/` with an `index.html` inside.
2. Add a button for it on the launcher page, `site/index.html`.
3. To remove a game, delete its folder and its button.

Each game is one self-contained HTML file, so you can copy Dino Dash and change it.

## How I host mine

Mine runs on Cloudflare's free plan, behind a login so only family can open it. `wrangler.jsonc` has the settings: it publishes the `site` folder on my own address only, with no other public links, and `site/robots.txt` keeps search engines out. Any static web host works just as well.

## What's in here

| Path | What it is |
|---|---|
| `site/index.html` | The launcher page |
| `site/games/` | One folder per game |
| `site/shared/fonts/` | The Baloo 2 font, shared by the games |
| `site/robots.txt` | Keeps search engines out |
| `wrangler.jsonc` | My Cloudflare settings |

## Licence

- The games and code: [MIT](LICENSE). Use them however you like.
- The Baloo 2 font: [SIL Open Font Licence](site/shared/fonts/OFL.txt).
