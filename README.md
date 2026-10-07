# The Marque Museum

A virtual museum of the automobile, built as a single web page. It's laid out like a real museum: wings by country, a room for each marque, and a placard for each car that explains what it is and why it matters — from the 1886 Benz Patent-Motorwagen to today's electric cars.

There are over 100 marques and more than 600 cars, each with its own short write-up, a photo, and a few key facts (engine, output, years made).

## Opening it

There's no build step and nothing to install. Open `marque-museum.html` in any web browser and the whole museum loads — home page, search, every car's page, a timeline view, all of it.

If you want to serve it locally instead of opening the file directly, any simple local server works, for example:

```
python3 -m http.server
```

then visit the page in your browser.

## What's in the project

- **`marque-museum.html`** — the whole site. One file: the page, its styling, and every car and marque's details.
- **`images/`** — a photo for most cars, downloaded in advance so the site works offline. Where no free photo exists, the page draws a simple illustration instead.
- **`audio/`** — one quiet instrumental track for the optional "gallery music" toggle in the header.
- **`fetch_photos.py`** — the script that originally found and downloaded the photos in `images/`. You don't need to run it to use the site; it's there if you ever want to refresh or re-fetch the photos.

## About the photos

Every photo comes from Wikimedia Commons and is freely licensed — nothing here needs permission to use. Each car's page credits its photographer and links back to the original on Commons. A handful of cars don't have a free photo available anywhere; those show a simple drawing instead, which was the plan from the start rather than a gap to fill in.

## About the music

The small toggle in the header plays a quiet jazz piano track in the background, off by default. It's in the public domain (CC0), credited in the footer. Browsers won't let a page play sound on its own, so it only starts once you click it.

## The writing

The history and facts on each placard were written for this project rather than copied from anywhere else.
