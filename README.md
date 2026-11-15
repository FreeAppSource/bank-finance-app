# Bank Finance App

> 👨‍💻 Developed by **[Suresh Kumar Meesala](https://github.com/SureshKumarMeesala)** · 🎨 UI design by **Peeely** (credits below)

A mobile app built with **React Native (0.88+)**, **Expo SDK 58+** and **Expo Router**, using **JavaScript and JSX (`.js`, `.jsx`)**. Every screen is built from the original Sketch design `bank-finance-app-uimates.sketch` by **Peeely**: one route per artboard, with the artboard's layout, colours, images and text.

![Bank Finance App screens](./showcase.jpg)

## 📱 Screens (7 design artboards)

Listed in the order of the app's flow. "Taps" is the number of tap targets wired on the screen (buttons, tabs, back arrows, list rows).

| # | Screen (artboard) | Route | Size | Taps |
|---|---|---|---|---|
| 1 | **Welcome** · start screen | `src/app/welcome.jsx` | 414 × 896 | 2 |
| 2 | **Onboarding 01** | `src/app/onboarding-01.jsx` | 414 × 896 | 2 |
| 3 | **Dashbaord** | `src/app/dashbaord.jsx` | 414 × 896 | 6 |
| 4 | **Onboarding 02** | `src/app/onboarding-02.jsx` | 414 × 896 | 2 |
| 5 | **Cards** | `src/app/cards.jsx` | 414 × 896 | 4 |
| 6 | **Earnings** | `src/app/earnings.jsx` | 414 × 896 | 5 |
| 7 | **Onboarding 03** | `src/app/onboarding-03.jsx` | 414 × 896 | 2 |

Screenshots of every screen are in [`screenshots/`](./screenshots).

## 🧩 How it's built

- `src/screens/*.json`: each design artboard converted to screen data (vector shapes, gradients, image fills, masks, shadows, blurs and rich text, positioned as in the design), plus its tap targets
- `src/sketch/SketchScreen.jsx`: draws a screen at the device's width with `react-native-svg`, native `Text`/`TextInput` and `expo-blur`, and handles navigation between screens
- `src/app/`: Expo Router routes, one per artboard (`index.jsx` opens the start screen)
- `assets/images/`: images used by the design

## 🛠️ Tech Stack

- **Framework**: React Native 0.88+ / Expo SDK 58+
- **Navigation**: Expo Router (file-based routing)
- **Language**: JavaScript & JSX (`.js`, `.jsx`)
- **Rendering**: `react-native-svg`, `expo-blur`
- **Fonts**: Google Fonts via `@expo-google-fonts` (Inter), standing in for the design's original fonts where those aren't free

<!-- run-locally:start -->

## ▶️ Run locally

```bash
npm install
npx expo start
```

Then press `i` for the iOS simulator, `a` for Android, or `w` for the web, or scan the QR code with Expo Go.

<!-- run-locally:end -->

<!-- developer:start -->

## 👨‍💻 Developer

This React Native app was developed by **Suresh Kumar Meesala**.

| | |
|---|---|
| Developer | [Suresh Kumar Meesala](https://github.com/SureshKumarMeesala) |
| GitHub | [@SureshKumarMeesala](https://github.com/SureshKumarMeesala) |
| Organization | [FreeAppSource](https://github.com/FreeAppSource) |
| Repository | <https://github.com/FreeAppSource/bank-finance-app> |

<!-- developer:end -->

---

<!-- design-credits:start -->

## 🎨 Design Credits

This app is based on the free **Finance Concept App** design by **Peeely**, downloaded from Sketch App Sources. All visual design credit goes to the designer. The screens are reproduced from the original Sketch file; fonts that aren't free are replaced with similar Google Fonts, so some details may differ slightly from the original.

| | |
|---|---|
| Designer | [Peeely](https://www.sketchappsources.com/contributor/peeely) |
| Original design | [Finance Concept App](https://www.sketchappsources.com/contributor/peeely) |
| Downloaded from | [Sketch App Sources](https://www.sketchappsources.com/free-source/4503-banking-app-screens-sketch-freebie-resource.html) |
| Dribbble | <http://www.dribbble.com/peeeli> |
| Twitter | <https://twitter.com/peeely> |
| Original file | `bank-finance-app-uimates.sketch` |
| License / usage | Not stated on the page. Free download; give credit (Sketch App Sources Terms). Confirm with the designer before commercial use. |

**Attribution:**

> UI design: "Finance Concept App" by Peeely (http://www.dribbble.com/peeeli), downloaded from Sketch App Sources (https://www.sketchappsources.com/free-source/4503-banking-app-screens-sketch-freebie-resource.html).

The original design source files are not included in this repository; get them from the links above. This app's **code** is released under the [MIT License](./LICENSE); the visual design remains the designer's (see [NOTICE](./NOTICE)).

Photos, brand logos and avatars inside the design may belong to third parties and are not covered by the designer's permission.

<!-- design-credits:end -->
