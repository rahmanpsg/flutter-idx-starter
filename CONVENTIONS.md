## Coding Guidelines for Flutter with Stacked Framework

### General Guidelines
- Follow the official [Flutter Style Guide](https://dart.dev/guides/language/effective-dart/style).
- Use descriptive and meaningful names for variables, methods, and classes.
- Break down large widgets and views into smaller, reusable components.
- Ensure code readability and maintainability.
- Write unit tests and widget tests for critical parts of the application.

### Stacked Framework
- Use `StackedViewModel` for the ViewModel classes.
- Separate business logic from UI code by placing it into ViewModels.
- Prefer using the `Stacked` package for state management.
- Use services, repositories, and managers for handling data, API calls, and business logic outside the ViewModel.

### Packages and Libraries
- Prefer `http` for HTTP requests, or use `dio` for more advanced HTTP client features.
- Use `stacked_generator` for generate view, service, bottom_sheet, dialog.

### State Management
- Use `Reactive` types in ViewModels to keep the UI updated.
- Use `Future` and `Stream` for asynchronous programming.

### Type Safety
- Use Dart's strong typing system and provide type annotations throughout the code.
- Avoid using `dynamic` and explicitly specify types wherever possible.

### Naming Conventions
- Use PascalCase for classes and enum names.
- Use camelCase for variable names, function names, and method parameters.
- Prefix private classes, methods, and variables with an underscore `_`.

### Comments and Documentation
- Add comments for complex logic and to describe the purpose of the code.
- Use Dart's documentation comments (`///`) to document public APIs, classes, and methods.
- Keep comments and documentation up to date with the code changes.

### Testing
- Write unit tests with the `test` package.
- Use `mockito` for mocking in tests.
- Write UI and integration tests using the `flutter_test` package.

### Performance
- Avoid unnecessary rebuilds by using the `notifyListeners()` method efficiently.
- Use the `const` keyword whenever possible to optimize the performance of the widgets.
- Profile and optimize the app using Flutter's dev tools.

### Additional Guidelines
- Modularize functionality by using separate dart files and folders.
- Keep widget-specific logic within the widget class itself and move shared logic to ViewModels.
- Use `FormBuilder` for form validation and management if required.