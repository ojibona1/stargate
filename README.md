# Stargate

Starlink roaming WISP. Zero-friction WiFi onboarding via captive portal — users connect, enter email, verify, and get internet. No app install, no MAC knowledge needed.

## Architecture

```
worker/        # Captive portal and auth Cloudflare Worker
  src/         # Routes and handlers
backend/       # Backend services
  src/         # Session management, billing
frontend/      # Next.js onboarding portal
  src/
data/          # D1 schemas
```

## Stack
Cloudflare Workers, WARP, Python, D1, Next.js, Tailwind
