# Flutter Customer Management App

A Flutter application demonstrating customer data management with theme switching capabilities.

## Features
- Customer list display with pagination
- Search functionality across customer records
- Light/Dark theme toggle
- Loading states with animated indicators
- Cross-platform support (Android, iOS, Web)

## Installation
```bash
flutter pub get
```

## Running the App
```bash
flutter run
```

## Key Dependencies
- provider: ^6.1.1 (State management)
- http: ^0.13.5 (API communication)
- shared_preferences: ^2.2.2 (Theme persistence)
- flutter_spinkit: ^5.1.0 (Loading animations)

## Project Structure
```
lib/
├── screens/           # UI screens
├── widgets/           # Reusable components
├── provider/          # State management
├── services/          # API communication layer
└── models/            # Data models
```

## Notes for Reviewers
1. State Management:
   - Uses Provider pattern for app state
   - CustomerProvider handles data loading/pagination
   - ThemeProvider manages dynamic theming

2. API Integration:
   - API service with base URL configuration
   - Error handling for network requests
   - Mockable pagination implementation

3. Key Widgets:
   - CustomerListItem: Custom list item with hover effects
   - LoadingIndicator: Animated spinkit integration
   - CustomSearchBar: Debounced search implementation

4. Testing:
   - Widget tests in test/widget_test.dart
   - CI/CD-ready structure
