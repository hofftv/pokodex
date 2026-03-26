# Pokopia Pokodex

A mobile-friendly reference app for **Pokémon Pokopia** (Nintendo Switch 2). Tap any uncaught Pokémon to see which habitats to build, what materials you need, and where to place them. Works offline from your phone's home screen.

## Features

- All 300 Pokémon with silhouette/color toggle for caught tracking
- 209 habitats with materials, rarity, locations, time, and weather data
- Tap any Pokémon to see which habitats attract it
- Tap a habitat card to see all Pokémon that appear there
- Filter by region (Bleak Beach, Cloud Island, Palette Town, Rocky Ridges, Sparkling Skylands, Withered Wastelands)
- Search by name, filter by caught/missing
- Alternate forms tracked independently (Pikachu/Peakychu, Shellos forms, etc.)
- Works offline (PWA with service worker)
- Boot-up animation because it's fun

## How to Use

1. Clone this repo
2. Deploy to Vercel: `npx vercel --yes --prod`
3. Open the URL on your phone and add to home screen
4. Tap Pokémon to look up habitats, mark them caught as you go

Your caught list saves locally in your browser — no accounts, no shared data.

## Data Source

All Pokémon and habitat data scraped from [Serebii.net](https://www.serebii.net/pokemonpokopia/). To update the data, run the scraper in `../scripts/`.

## Tech

Zero dependencies, zero build step. One HTML file + one data file + service worker.
