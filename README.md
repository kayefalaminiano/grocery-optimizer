# Grocery Optimizer (Mobile + API + DB)

A mobile app that compares a shopping list across nearby stores and returns the cheapest option with a price breakdown.

## Tech Stack
- **Mobile:** React Native (Expo)
- **API:** Node.js + Express
- **Database:** Postgres (planned) / Hardcoded seed data (current)

## Architecture
- `mobile/` handles UI + state and calls the API
- `server/` exposes a REST endpoint for comparison logic
- (Later) Postgres stores products, stores, and prices


## Current Features
- Enter location (ZIP)
- Build a shopping list (items + quantities)
- Compare store totals and rank cheapest → most expensive
- Handles missing prices (shows item as unavailable / skips based on rules)

## Roadmap
- [ ] Replace hardcoded seed data with Postgres
- [ ] Product search endpoint
- [ ] Unit price normalization (oz/lb/each)
- [ ] Price history tracking + charts
- [ ] Split-basket optimization

## Getting Started

### Mobile
```bash
cd mobile
npm install
npx expo start



