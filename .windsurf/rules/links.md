---
trigger: model_decision
description: Apply this rule whenever creating or modifying screens, navigation, theming, accessibility, or build/test flows in this Expo Router app to enforce Apple/shadcn style, safe-area/deep-link conventions, and our documented tokens and components.
---

# 📚 Links & Rationale (Expo Router + Apple/shadcn aesthetic)

> Use these sources when implementing or reviewing UI, navigation, performance, builds, accessibility, and tests. Each link lists **how and where** we use it in this codebase so prompts can reference the right authority.

---

## 1) Apple Design System (HIG) & Assets

- Human Interface Guidelines (HIG)  
  https://developer.apple.com/design/human-interface-guidelines/  
  _Use for_: overall principles, layout, motion, color, and platform conventions.  
  _Where we apply_: `docs/context/10_UI_FOUNDATIONS.md`, `11_COMPONENT_STANDARDS.md`.

- UI Design Do’s & Don’ts  
  https://developer.apple.com/design/tips/  
  _Use for_: quick polish checks, before screenshots/PRs.  
  _Where we apply_: PR template “Design QA” checklist.

- Typography / Color / Motion / Layout / Writing / Inclusion  
  https://developer.apple.com/design/human-interface-guidelines/typography  
  https://developer.apple.com/design/human-interface-guidelines/color  
  https://developer.apple.com/design/human-interface-guidelines/motion  
  https://developer.apple.com/design/human-interface-guidelines/layout  
  https://developer.apple.com/design/human-interface-guidelines/writing  
  https://developer.apple.com/design/human-interface-guidelines/inclusion/  
  _Use for_: token definitions, animation decisions, microcopy tone.  
  _Where we apply_: `10_UI_FOUNDATIONS.md` (tokens), `80_COPYWRITING_TONE.md`.

- Apple Design Resources (Figma kits, templates)  
  https://developer.apple.com/design/resources/  
  _Use for_: aligning spacing/typography and assets to Apple defaults.

- SF Symbols / Apple Fonts  
  https://developer.apple.com/sf-symbols/  
  https://developer.apple.com/fonts/  
  _Use for_: iconography and type pairing guidelines.

---

## 2) Accessibility & Inclusive Design

- Apple Accessibility (developer hub)  
  https://developer.apple.com/accessibility/  
- HIG – Accessibility & Inclusion (see links above)  
- WCAG 2.2 Quick Reference (W3C)  
  https://www.w3.org/WAI/WCAG22/quickref/  
  _Use for_: VoiceOver labels, minimum hit areas (≥44×44), dynamic type, contrast.  
  _Where we apply_: `12_ACCESSIBILITY_IOS.md`, component checklists in `11_COMPONENT_STANDARDS.md`.

---

## 3) Expo Router, Linking & Deep Links

- Expo Router – Introduction / Installation  
  https://docs.expo.dev/router/introduction/  
  https://docs.expo.dev/router/installation/  
- Linking overview / API / “Into other apps”  
  https://docs.expo.dev/linking/overview/  
  https://docs.expo.dev/versions/latest/sdk/linking/  
  https://docs.expo.dev/linking/into-other-apps/  
  _Use for_: file-based routing, nested stacks/tabs, deep links & Universal Links.  
  _Where we apply_: `docs/context/20_NAVIGATION_MAP.md`.

---

## 4) UI Chrome & Safe Areas (edge-to-edge)

- `react-native-safe-area-context` (Expo docs)  
  https://docs.expo.dev/versions/latest/sdk/safe-area-context/  
- StatusBar (`expo-status-bar`)  
  https://docs.expo.dev/versions/latest/sdk/status-bar/  
- System bars (edge-to-edge guidance)  
  https://docs.expo.dev/develop/user-interface/system-bars/  
  _Use for_: notch/home-indicator spacing, status bar behavior, immersive layouts.  
  _Where we apply_: screen layouts and `app/_layout.tsx`.

---

## 5) Build, Ship & OTA

- EAS Build – setup / development builds / `eas.json`  
  https://docs.expo.dev/build/setup/  
  https://docs.expo.dev/develop/development-builds/create-a-build/  
  https://docs.expo.dev/build/eas-json/  
- `expo-updates` + OTA updates  
  https://docs.expo.dev/versions/latest/sdk/updates/  
  https://docs.expo.dev/deploy/send-over-the-air-updates/  
- App Store submission (Apple)  
  https://developer.apple.com/ios/submit/  
  _Use for_: CI profiles, runtime versions, channels, store submission checklists.  
  _Where we apply_: `70_SECURITY_AND_SECRETS.md`, `docs/release/RELEASE_CHECKLIST.md`.

---

## 6) Performance Essentials

- React Native – Performance overview  
  https://reactnative.dev/docs/performance  
- Hermes JS engine (RN docs)  
  https://reactnative.dev/docs/hermes  
- FlatList (virtualization)  
  https://reactnative.dev/docs/flatlist  
  _Use for_: cold-start targets, list virtualization, memory budgets, Hermes defaults.  
  _Where we apply_: `60_PERFORMANCE_BUDGETS.md`.

---

## 7) “shadcn-ish” foundations for React Native

- shadcn/ui (concepts & theming)  
  https://ui.shadcn.com/do
