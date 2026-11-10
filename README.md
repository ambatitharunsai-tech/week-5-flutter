# Flutter Week 5 – State Management

Two examples comparing local widget state with shared application state using the Provider package.

## Exercises

| File | Description |
|---|---|
| `5(A)` | Stateful switch that updates its value and displays whether it is ON or OFF |
| `5(B)` | Counter comparison: one counter uses `setState`, while another uses `ChangeNotifier` and `Provider` |
| `output_5a.jpeg`, `output_5b.jpeg` | Screenshots of the exercise outputs |

## Concepts covered

- `StatefulWidget` and `setState`
- Handling a `Switch` value with a callback
- Creating a `ChangeNotifier` model
- Calling `notifyListeners()` after state changes
- Providing shared state with `ChangeNotifierProvider`
- Reading state from widgets with Provider

## Run the examples

This repository stores the exercises as extensionless Dart files rather than a complete Flutter project.

```bash
flutter create state_management_demo
cd state_management_demo
```

For exercise `5(A)`, copy the source into `lib/main.dart`. For `5(B)`, add Provider to the generated project's dependencies:

```bash
flutter pub add provider
```

Then copy the relevant source into `lib/main.dart` and run `flutter run`.

## When to use each approach

Use `setState` for state that belongs to one widget. Use a shared state solution such as Provider when multiple widgets need to observe and react to the same state.
