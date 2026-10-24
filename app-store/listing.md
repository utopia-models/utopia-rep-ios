# Utopia Rep — App Store Connect listing, first submission

Pasted into App Store Connect field by field once the app record exists (`../README.md`, step 3).

| field | value |
|---|---|
| Name | Utopia Rep |
| Subtitle | Door map, quotes and booking |
| Bundle id / SKU | `com.utopiacleans.rep` / `utopia-rep` |
| Primary category | Business |
| Secondary category | Productivity |
| Age rating | 4+ (every questionnaire answer "None") |
| Price | Free |
| Distribution | Unlisted app distribution: reps install it from a direct link and it never appears in search or charts. Requested after the first approval, at developer.apple.com/contact/request/unlisted-app |
| Support URL | `https://utopiacleans.com` |
| Marketing URL | `https://utopiacleans.com` |
| Copyright | 2026 Utopia Models, Inc. |

## Promotional text

See every house on your route, its price and its status before you knock.

## Description

Utopia Rep is the field app for Utopia Cleans sales reps in Colorado Springs.

- A map of the doors in your territory, each pinned with its status: not knocked, not home, follow up, booked.
- One tap at the door records the outcome where you are standing. No signal? It is saved on the phone and sends when you reconnect.
- Type an address to see the price and the house facts before you knock, then book the clean on the spot.
- Take a photo of the house or the door and it is saved with the visit.
- Get a notification when a house you knocked books, and when it is time to go back to a follow-up.
- Track the houses you closed and what you have earned.

Sign-in is by a text code sent to the phone number on your rep account.

## Keywords

door to door,canvassing,sales,field sales,route,cleaning,quotes,booking,leads,map

## What the app does natively (guideline 4.2)

Push notifications through APNs when a knocked house books or a follow-up is due; the native camera for house
and door photos; the device location to center the map and pin the knock; an offline page that resumes the app
when signal returns. Write this paragraph into *Notes* for App Review together with the sign-in below.

## App Review sign-in

The app signs in by a text code, so the review needs a demo rep: a rep row whose phone number and code are
fixed, given in *Sign-in required* → user name (the phone number) and password (the code). The rep app
(utopia-models/knowledge#9977) creates that account before the first submission; its values are stored in Infisical as
`utopia/CLEANING_APP_REVIEW_PHONE` and `utopia/CLEANING_APP_REVIEW_CODE`, never in this file.

## App Privacy answers

Data used to track you: none. Data linked to you, all for *App Functionality*: Contact Info → Name, Phone
Number; Location → Precise Location; User Content → Photos; Identifiers → User ID. No third-party analytics
or advertising SDK is in the app.

## Screenshots

6.9-inch iPhone (1320 × 2868), three to five: the door map, a quote for an address, the booking confirmation,
earnings. Captured from the simulator build (`ios` workflow artifact) once slices A and B are live.

## Not yet in place

App Store Connect will not submit without a **Privacy Policy URL**, and `utopiacleans.com` has none
(`/privacy` and `/privacy-policy` both return 404, 2026-10-24). Writing that page is legal content and is
outside this work (the Cleaning portfolio's README in utopia-models/knowledge).
