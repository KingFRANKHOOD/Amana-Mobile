# Amana-Mobile

This repository is the dedicated mobile client for the Amana escrow protocol, built with React Native and Expo.

## Tech Stack

- **Framework**: React Native with Expo
- **Language**: TypeScript
- **Navigation**: React Navigation (stack-based)
- **State Management**: Zustand for lightweight store management
- **Wallet**: Stellar Freighter integration
- **Notifications**: Expo Push Notifications / Firebase Cloud Messaging
- **Secure Storage**: Expo Secure Store for token persistence
- **Code Quality**: ESLint, Prettier, TypeScript strict mode

## Features

- Wallet-based authentication via Stellar
- Trade discovery and status tracking
- Evidence capture and upload
- Real-time push notifications for trade events
- Secure token storage on device
- Offline-aware state management

## Getting Started

### Prerequisites

- Node.js 20+ / npm or yarn
- Expo CLI: `npm install -g expo-cli`
- iOS Simulator (on macOS) or Android Emulator

### Install dependencies

```bash
cd Amana-Mobile
npm install
```

### Environment

Copy the example env file:

```bash
cp .env.example .env.local
```

Configure for your environment:
- `EXPO_PUBLIC_API_URL` – backend API endpoint (default: http://localhost:4000)
- `EXPO_PUBLIC_STELLAR_NETWORK` – testnet or public network
- `EXPO_PUBLIC_PUSH_PROVIDER` – expo or firebase

### Run in development

```bash
npm start
```

Then select:
- `i` for iOS Simulator
- `a` for Android Emulator
- `w` for web (requires `expo-web`)

### Build for production

```bash
npm run build
```

### Type check

```bash
npm run type-check
```

### Lint

```bash
npm run lint
```

## Project structure

- `src/api/` – API client and service methods
- `src/stores/` – Zustand state management
- `src/screens/` – Screen components
- `src/App.tsx` – Root app component
- `app.config.ts` – Expo configuration
- `docs/mobile.md` – Mobile environment specifications

## Backend integration

See `docs/mobile.md` for mobile API requirements and environment setup.

## Notes

- The mobile app uses the same backend authentication and trade services as the web application.
- Payloads are optimized for low-bandwidth mobile environments.
- Secure token storage prevents credentials from being logged or exposed.
