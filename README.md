# Expense Tracker

## About the Project

Expense Tracker is an Android application for managing personal expenses. The application allows users to view, add, search, and filter expenses.

## Features

- View a list of expenses
- Add a new expense
- Search expenses by name
- Filter expenses by category
- View expense details
- Add or remove an expense from favorites
- Switch between light and dark themes

## Screens

The application has three main screens:

1. **Home Screen** — displays the total expenses, categories, search field, and a list of recent expenses.
2. **Expense Details Screen** — displays detailed information about a selected expense.
3. **Add Expense Screen** — allows the user to add a new expense.

## Technologies

- Kotlin
- Jetpack Compose
- Material 3
- Navigation Compose

## Architecture

The application uses a simple layered architecture:

UI → ViewModel → Repository

### UI Layer

The UI layer contains the screens and composables in `MainActivity.kt`.

`HomeScreen()` receives `HomeUiState` and callback functions. It does not directly access the `HomeViewModel`.

`HomeRoute()` connects the UI with the ViewModel and collects the state using `collectAsStateWithLifecycle()`.

### ViewModel Layer

`HomeViewModel.kt` contains `HomeViewModel` and manages the application state.

It uses a private `MutableStateFlow` and exposes a public `StateFlow<HomeUiState>`.

The ViewModel handles user actions such as:

- searching expenses;
- selecting a category;
- adding a new expense;
- adding or removing an expense from favourites.

State is updated using `copy()`.

### Repository Layer

`ExpenseRepository.kt` owns the expense data.

It provides functions for loading expenses, adding a new expense, and changing the favourite status.

The repository uses `delay()` to simulate data loading and can simulate a loading error.

## Rotation

When the device rotates, `MainActivity` is recreated, but `HomeViewModel` survives the configuration change.

Because the UI state is stored in the ViewModel, the search query, selected category, and favourite expenses remain after rotation.

Lifecycle logs show that the Activity is recreated during rotation, while `HomeViewModel` is not created again.

## Project Structure

- `MainActivity.kt` — contains the main application logic, screens, navigation, and reusable components.
- `ui/theme/Color.kt` — contains custom colors for the application.
- `ui/theme/Theme.kt` — configures the light and dark themes.

## Screenshots

### Light Theme

![Light Theme](screenshots/light_theme.png)

### Dark Theme

![Dark Theme](screenshots/dark_theme.png)