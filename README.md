# GrowPracticeApp

GrowPracticeApp is a blank SwiftUI starter project for your personal growth and practice. The idea is to build a stock broking app experience inspired by apps like Groww, but the project intentionally starts empty so you can design and implement every screen yourself.

This repo is not a trading product, does not connect to real stock exchanges, and does not include real payment or broker integrations. Treat it as a UI, architecture, and iOS practice playground.

## What Is Included

- A minimal iOS SwiftUI app target.
- A blank `ContentView`.
- An `Assets.xcassets` catalog with starter color tokens.
- Empty media placeholders for logo and illustrations.
- A detailed product and development plan in `PROJECT_PLAN.md`.

## What Is Not Included

- No login implementation.
- No stock list implementation.
- No details screen implementation.
- No payment gateway implementation.
- No portfolio or holdings implementation.
- No API layer, database layer, or state management.

The goal is to give you a clean project that opens and runs, while leaving the real development work for your own practice.

## App Idea

Build a stock broking practice app with the following user journey:

1. User opens the app.
2. User logs in through an offline/mock login screen.
3. User sees a list of stocks.
4. User searches and filters stocks.
5. User opens a stock details page.
6. User starts a mock buy flow.
7. User completes a simulated payment.
8. User sees a bought stocks / holdings status page.
9. User compares bought price with current price.

## Suggested Screens

### Offline Login

Purpose: practice forms, validation, state handling, and navigation.

Possible fields:

- Email or mobile number
- Password or PIN
- Login button
- Error state
- Loading state
- Demo user hint

Practice goals:

- Form validation
- Secure text input
- Basic local authentication state
- Clean visual hierarchy

### Stock Listing

Purpose: practice lists, search, filtering, and reusable cells.

Possible content:

- Stock symbol
- Company name
- Current price
- Daily change
- Watchlist button

Practice goals:

- `List`, `ScrollView`, or custom lazy stacks
- Search bar behavior
- Empty states
- Loading and error states
- Cell component extraction

### Stock Details

Purpose: practice detail pages and richer product UI.

Possible content:

- Company name and symbol
- Current price
- Price movement
- Simple chart placeholder
- Buy button
- About company section
- Key metrics section

Practice goals:

- Detail layout composition
- Charts or chart placeholders
- Sectioned content
- Navigation from list to detail

### Payment Gateway

Purpose: practice multi-step flows without using real payment APIs.

Possible content:

- Selected stock
- Quantity
- Estimated order value
- Payment method selection
- Confirm button
- Success / failure state

Practice goals:

- Form state
- Confirmation screens
- Mock async operations
- Error handling

### Bought Stocks Status

Purpose: practice portfolio-style UI and derived calculations.

Possible content:

- Stock symbol
- Quantity bought
- Bought price
- Current price
- Profit / loss amount
- Profit / loss percentage

Practice goals:

- Local models
- Derived values
- Sorting holdings
- Green/red visual states

## Asset Catalog

The starter project includes these color placeholders:

- `BrandPrimary`
- `BrandSecondary`
- `ScreenBackground`
- `ProfitGreen`
- `LossRed`

The starter project includes these empty media placeholders:

- `Logo`
- `LoginIllustration`
- `EmptyPortfolio`

You can replace the empty image sets later with your own PNG, PDF, or SVG-exported assets.

## Suggested Folder Structure To Add Later

As you build the app, consider growing the project gradually:

```text
GrowPracticeApp/
  App/
  Features/
    Login/
    Stocks/
    StockDetails/
    Payment/
    Holdings/
  Shared/
    Components/
    Models/
    Services/
    Theme/
```

Do not create all folders too early. Add each folder when you actually start building that feature.

## Practice Rules

- Keep the first version offline.
- Use fake data first.
- Build one screen at a time.
- Commit after each milestone.
- Avoid copying real app assets or branding.
- Use your own app name, colors, and layout decisions.

## Running The App

1. Open `GrowPracticeApp.xcodeproj` in Xcode.
2. Select an iPhone simulator.
3. Run the app.
4. You should see a blank screen.

That blank screen is intentional. Start by designing your login screen in `ContentView.swift` or by creating a new feature folder when you are ready.
