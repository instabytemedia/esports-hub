# Esports Hub

> Game on with Crypto Stadium

This variant focuses on the esports community, allowing professional gamers to create and trade unique digital collectibles, such as in-game items and exclusive skins. Fans can participate in prediction markets for upcoming matches and engage in AR-powered fantasy leagues. The platform will partner with popular esports teams and leagues to offer exclusive content.

## Features

- Digital collectible marketplace
- Prediction markets
- AR-powered fantasy leagues

## Tech Stack

- **Framework:** Next.js 15 (App Router)
- **Database:** Supabase (PostgreSQL)
- **Auth:** Supabase Auth
- **Styling:** Tailwind CSS
- **Language:** TypeScript

## Getting Started

1. Clone this repository
2. Copy `.env.example` to `.env.local` and fill in your credentials
3. Run `npm install`
4. Run `npm run dev`

## Project Structure

```
├── app/                  # Next.js App Router pages
├── components/           # React components
├── lib/                  # Utilities and helpers
├── supabase/            # Database schema
└── INSTRUCTIONS.md      # Detailed build guide for AI assistants
```

## Database

This project uses 3 main entities:
- **Idea**: A concept or proposal for a new digital collectible, prediction market, or AR-powered fantasy sports league
- **Crypto**: A cryptocurrency used for transactions on the platform
- **Stadium**: A virtual stadium where users can participate in AR-powered fantasy sports leagues

## Build Instructions

For detailed step-by-step build instructions, see [`INSTRUCTIONS.md`](./INSTRUCTIONS.md).

This file contains comprehensive guidance for building this project with AI coding assistants like Claude Code, Cursor, or Windsurf.

---

*Generated with [Claudery](https://claudery.io) - AI-powered blueprint generator*
