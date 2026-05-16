# Amana-Mobile

This repository is the dedicated mobile client for the Amana escrow protocol.

## Vision

The mobile app should deliver a lightweight, touch-first experience for buyers, sellers, drivers, and mediators.
It should support trade creation, status tracking, evidence capture, dispute management, and real-time notifications.

## Recommended stack

- React Native with Expo
- TypeScript
- Expo Push Notifications or Firebase Cloud Messaging
- Secure device storage for tokens
- Offline-aware sync for intermittent connectivity

## Current status

This repo is currently a placeholder. The mobile backend contract and API requirements are defined in the backend repository.

## Mobile environment setup

Mobile environment configuration is available inside this repository.

- `docs/mobile.md` contains the mobile environment setup and API requirements.
- `.env.mobile.example` contains the mobile runtime variable template.

## Getting started

When the mobile client is added, use the following initial setup:

```bash
cd Amana-Mobile
npm install
```

Then configure mobile support by copying the mobile environment example into the mobile repo:

```bash
cp .env.mobile.example .env.mobile
```

## Notes

The mobile client should use the backend authentication and trade services while keeping payloads optimized for low-bandwidth mobile users.
