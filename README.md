# Bookstack Reading List React Native App

## Status and Demo

tbd.

### Tech Stack:

![Expo](doc/img/Expo.png)
![React](doc/img/React.svg)
![Radon](doc/img/Radon.png)
![Uniwind](doc/img/Uniwind.png)
![TypeScript](doc/img/TypeScript.svg)
![Storybook](doc/img/Storybook.svg)
![Storybook](doc/img/Jest.png)

- React Native + Uniwind + TypeScript
- Radon + VS Code + npm
- Storybook + Jest

## Notes

TODO order and clean up the notes below.

Further reading: [Apple App Store, TestFlight, Virtual Mac for App Development](https://github.com/openmindculture/tools-settings/blob/main/techtips/apple-test-flight-virtual-mac.md) 🍏

### App Idea: Book Grid Native

BookGrid TBR too be read wie SUB Stapel ungelesener Bücher, Keywords auch book tracking apps

https://github.com/openmindculture/bookstack-native-app

Expo app: A reading list app, native for Apple and Android, privacy-first local storage only, scanning ISBN barcode and location, if turned on, all presented in a hexgonal grid with a slightly retrofuturistic synthwave indie gamer aesthetic similar to the devux-bookstack web app, but extend the hexa grid tiled visually over the edges of the screen. Every time you scan a book, it spawns as a new tile on an infinite, zoomable hexagonal grid.

This specific combination of a local-first privacy model, spatial context mapping, and a heavy synthwave/indie-game aesthetic represents an completely empty niche in the current app marketplace. Existing book trackers focus on corporate, clean, flat, and productivity-driven UI designs.

####  The Core Unique Value Proposition (UVP)

Instead of treating reading like a chore, a checklist, or a social network, your app treats a personal reading list like an in-game inventory or an evolving map in a retro-cyberpunk RPG.

Visual States: Unread books have a "locked" dim overlay or static interference effect. Active books pulse with a subtle neon glow. Completed books turn into solid, retro-gold or chrome geometric icons.

Audio FX: Optional 8-bit or low-fi synth chimes when an ISBN barcode successfully scans or when a "hex" is completed.

#### 3. Retro "Data-Log" Geotagging
How it works: When location permissions are granted, scanning a book tags it with the local coordinates.
The Feature: The app displays this data using retro terminal styling (e.g., LOC: 52.4731° N, 13.4452° E // NEUKÖLLN). Tapping the coordinate pops open a wireframe mini-map inside the app showing exactly where you discovered that specific piece of "data" (the book).

## React Native Vega vs. Expo

Techtips + takeaways from React Berlin Meetup in May 2026:

- Vega vs Expo
- react-native-web
- no css grid (not real css)
- RLS role level security 
- supabase
- shadcn
- ORPC
- Tanstack
- storage: AsyncStorage + Zustand locally
- `npx expo start`
- CNG `app.json` smoother updates
- credential management: cred mgmt expo deploy to app stores
- AI mcp not for native yet
- app store optimization seemed easier than web SEO
- everybody has AI FOMO in 2026

### React Native / Expo vs Flutter?

AI answer: as of 2026, the old "JavaScript Bridge" is dead. React Native’s New Architecture (Fabric/JSI) is the default, giving you native-level performance that rivals Flutter for 90% of use cases.

####  AI: Why Flutter might be your "Power Move"

Flutter is the better choice only if your goal is to break away from the "web look" entirely or if you want to target Desktop/Embedded systems (like car dashboards or kiosks) alongside mobile.

Pixel Perfection: Because Flutter uses its own rendering engine (Impeller), an app looks exactly the same on a 2018 Android as it does on a 2026 iPhone.

Flutter is often cited as the best framework for vibe coding. Dart’s strict type system catches AI hallucinations instantly at compile-time, whereas JS/TS might fail at runtime.

### Astro to Expo

#### 1. App Dev

Starting fresh with Expo is the industry standard for React developers moving into mobile. It provides a "vibe-coding" friendly environment because of its extensive pre-configured tooling and high-quality documentation, which LLMs can parse effectively to generate working boilerplate.

Market Value: In 2026, companies prioritize "Cross-Platform" over "Web-Only." React Native is consistently ranked higher in job descriptions than PWA or Capacitor-only roles.

"Real App" Features: You will learn native patterns like Navigation stacks (Expo Router), Push Notifications, and Biometrics (FaceID/Fingerprint), which are often clunky or impossible in a pure web environment.
Developer Experience: Expo's "Fast Refresh" and the ability to test on your actual phone via the Expo Go app provide the instant feedback loop required for successful vibe coding.

#### 2. The Project: "Local-First" Utility

Avoid the "Todo List" trap. To impress recruiters and learn core app architecture, build a Local-First Expense Tracker or Habit Builder with the following native features:
- SQLite/WatermelonDB: Move beyond localStorage to learn proper mobile data persistence and sync.
- Native Gestures: Implement swipe-to-delete or pull-to-refresh using react-native-gesture-handler.
- Camera/Media Library: Allow users to snap a photo of a receipt or set a profile picture.
- Background Tasks: Trigger a local notification if a daily goal hasn't been met.

#### 3. Comparing the Architecture

Understanding the difference between your current web skills and the app landscape is crucial for your career transition.

Feature
- Astro + Capacitor (Option A)
- Expo / React Native (Option B)
- UI Components
- HTML/CSS (Webview)
- Native UI Views (Kotlin/Swift)
- Performance
- Good (Browser-level)
- Excellent (Native-level)
- Vibe Ease
- Very High (Standard Web)
- High (Expo simplifies native complexity)

Job Demand
- Niche/Specialized
- High/Universal
- Access to APIs
- Bridge-based (Capacitor)
- First-class/Native

#### 4. Implementation Steps for a Web Developer
Initialize: Run npx create-expo-app@latest to get the React 19-ready structure.
Navigation: Use Expo Router. It mimics file-based routing (like Astro/Next.js), making the transition intuitive.
Styling: Shift from CSS to StyleSheet or use NativeWind (Tailwind for React Native) to leverage your existing frontend skills.
Deployment: Use EAS (Expo Application Services) to build .ipa or .apk files without needing to open Xcode or Android Studio.

#### Authoritative Sources

https://reactnative.dev/architecture/overview
https://docs.expo.dev/router/introduction/
https://capacitorjs.com/docs/basics/vs-react-native
https://medium.com/effortless-programming/how-to-learn-to-build-apps-in-2025-2293d340886b
https://www.mol-tech.us/blog/progressive-web-apps-vs-native-apps-2026

