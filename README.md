# eOPS Platform - Esports Operations Platform

A comprehensive web application for managing esports organizations, teams, scrimmages, and player performance.

## Features

### Role-Based Access Control
- **Owner**: High-level oversight of all teams and organizational health
- **Manager**: Daily operations, scrim scheduling, and roster management
- **Coach**: Performance analysis, match reviews, and player statistics
- **Player**: Schedule visibility, availability management, and personal stats

### Key Functionality
- Scrim management and scheduling
- Player availability tracking
- Performance analytics and statistics
- Match reviews and coaching notes
- Team and game management
- Announcements system

## Tech Stack

- **React 18** with TypeScript
- **Vite** for build tooling
- **React Router** for navigation
- **Lucide React** for icons
- Modern CSS with custom design system

## Getting Started

### Prerequisites
- Node.js 18+ and npm/yarn

### Installation

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Open your browser to `http://localhost:3000`

### Demo Accounts

You can log in with any of these demo accounts:
- `owner@eops.com` - Team Owner
- `manager@eops.com` - Team Manager
- `coach@eops.com` - Team Coach
- `player@eops.com` - Player

(Password can be anything for demo purposes)

## Project Structure

```
src/
├── components/        # Reusable UI components
│   └── Layout/       # Layout components (Sidebar, Header, etc.)
├── context/          # React context providers
├── data/             # Mock data
├── pages/            # Page components
│   ├── Auth/         # Authentication pages
│   ├── Owner/        # Owner-specific pages
│   ├── Manager/      # Manager-specific pages
│   ├── Coach/        # Coach-specific pages
│   └── Player/       # Player-specific pages
├── styles/           # Global styles and design system
└── types/            # TypeScript type definitions
```

## Design System

The platform uses a consistent design system with:
- Dark theme optimized for extended use
- Color-coded availability indicators
- Responsive grid layouts
- Accessible components following WCAG 2.1 Level AA guidelines

## Build

To build for production:
```bash
npm run build
```

To preview the production build:
```bash
npm run preview
```

## License

This project is created for demonstration purposes.

