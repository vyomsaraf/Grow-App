# GrowPracticeApp Project Plan

## Goal

Build a personal iOS practice app that simulates the core experience of a stock broking app. The app should help you practice SwiftUI, navigation, state management, forms, lists, search, detail pages, mock payments, and portfolio calculations.

The first version should remain fully offline and should use mock data only.

## Guiding Principle

Start blank. Build slowly. Each milestone should teach one skill clearly.

Avoid building too many abstractions at the beginning. Add structure only when a feature needs it.

## Phase 0: Project Setup

Status: starter project created.

Included:

- Blank SwiftUI app.
- Blank `ContentView`.
- Starter colors in asset catalog.
- Empty media placeholders.
- README and project plan.

Your next task:

- Open the project in Xcode.
- Run the blank app.
- Decide the app name, theme, and first screen layout.

## Phase 1: Offline Login

Objective: create the first screen and basic offline access flow.

Build:

- Login screen UI.
- Email or mobile field.
- Password or PIN field.
- Login button.
- Basic validation.
- Error message for empty or invalid fields.
- Successful login state.

Recommended fake login:

- Email: `demo@growpractice.app`
- Password: `password`

Skills practiced:

- SwiftUI forms.
- Local state with `@State`.
- Input validation.
- Conditional UI.
- Moving from one app state to another.

Completion checklist:

- User cannot continue with empty fields.
- User sees a clear error message.
- User can log in with demo credentials.
- User lands on the next area of the app after login.

## Phase 2: App Navigation

Objective: create the main app structure after login.

Build:

- A main screen after login.
- Navigation container.
- Tabs or simple navigation links.
- Placeholder destinations for stocks and holdings.

Suggested navigation:

- Stocks
- Holdings
- Profile or Settings later

Skills practiced:

- `NavigationStack`.
- `TabView`.
- App-level state.
- Deciding feature boundaries.

Completion checklist:

- Login changes the root app state.
- Main area has a clear structure.
- Empty placeholders exist only where you need them next.

## Phase 3: Stock Listing

Objective: show a searchable list of mock stocks.

Build:

- Local `Stock` model.
- Mock stock data.
- List row UI.
- Search by company name or stock symbol.
- Empty state when search has no results.

Suggested stock fields:

- Symbol
- Company name
- Current price
- Daily change amount
- Daily change percentage

Skills practiced:

- Models.
- Mock data.
- Lists.
- Search.
- Filtering.
- Reusable row views.

Completion checklist:

- Stocks appear in a list.
- Search filters results.
- Empty search result is handled.
- Row UI is clean and readable.

## Phase 4: Stock Details

Objective: create a detail page for one selected stock.

Build:

- Header with stock name and symbol.
- Current price.
- Price change.
- Chart placeholder.
- About section.
- Buy button.

Optional additions:

- Key metrics.
- 52-week high / low.
- Market cap.
- Watchlist action.

Skills practiced:

- Navigation from list to detail.
- Passing model data between screens.
- Sectioned layouts.
- Scrollable detail pages.

Completion checklist:

- Tapping a stock opens detail.
- Detail screen shows the selected stock.
- Buy button is visible.
- Layout works on different iPhone sizes.

## Phase 5: Mock Payment Flow

Objective: simulate buying a stock without real payment integration.

Build:

- Quantity selector.
- Order summary.
- Mock payment method selection.
- Confirm button.
- Loading state.
- Success state.
- Failure state if you want extra practice.

Important:

- Do not connect a real payment gateway for this practice version.
- Use a fake delay to simulate processing.

Skills practiced:

- Multi-step flow.
- Form state.
- Derived totals.
- Mock async behavior.
- Success and failure UI.

Completion checklist:

- User can select quantity.
- App calculates estimated total.
- User can simulate payment.
- Success screen appears after confirmation.

## Phase 6: Bought Stocks / Holdings

Objective: show stocks the user has bought and compare bought price with current price.

Build:

- Local `Holding` model.
- Store completed mock purchases.
- Holdings list.
- Bought price.
- Current price.
- Profit / loss amount.
- Profit / loss percentage.

Suggested derived values:

```swift
currentValue = currentPrice * quantity
investedValue = boughtPrice * quantity
profitLoss = currentValue - investedValue
profitLossPercentage = profitLoss / investedValue * 100
```

Skills practiced:

- Shared app state.
- Derived calculations.
- Local portfolio model.
- Formatting currency and percentages.
- Positive and negative visual states.

Completion checklist:

- Bought stock appears in holdings.
- Bought price is shown.
- Current price is shown.
- Profit and loss are calculated correctly.
- Profit uses green, loss uses red.

## Phase 7: Polish

Objective: improve product quality and presentation.

Build:

- App theme.
- Consistent spacing.
- Reusable buttons.
- Loading states.
- Empty states.
- Error states.
- App icon.
- Launch screen polish.

Skills practiced:

- Design systems.
- Asset usage.
- Reusable SwiftUI components.
- Visual consistency.

Completion checklist:

- App looks consistent.
- Colors are pulled from assets.
- Reusable components reduce duplication.
- Empty and error states feel intentional.

## Phase 8: Optional Advanced Practice

Choose any of these when the main app is complete:

- Persist holdings locally with `UserDefaults`, SwiftData, or files.
- Add watchlist support.
- Add a fake API service layer.
- Add charts.
- Add sorting and filters.
- Add unit tests for calculations.
- Add snapshot tests for major screens.
- Add accessibility labels.
- Add dark mode polish.
- Add localization.

## Suggested Commit Plan

1. `Create blank SwiftUI starter`
2. `Add offline login screen`
3. `Add main navigation shell`
4. `Add stock list with mock data`
5. `Add stock search`
6. `Add stock details screen`
7. `Add mock payment flow`
8. `Add holdings status screen`
9. `Add portfolio profit loss calculations`
10. `Polish theme and assets`

## Suggested Learning Focus

For each feature, write down:

- What SwiftUI concept did I practice?
- What was difficult?
- What would I improve if this were a production app?
- What should I refactor later?

This will make the project useful for interviews, personal growth, and future GitHub portfolio work.
