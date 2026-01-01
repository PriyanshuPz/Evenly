# Contributing to Evenly

Thank you for your interest in contributing to Evenly! This guide will help you get started.

## Prerequisites

- **Flutter SDK** (3.9.2 or compatible) - [Install Flutter](https://flutter.dev/docs/get-started/install)
- **Dart SDK** (comes with Flutter)
- **IDE**: VS Code, Android Studio, or IntelliJ IDEA with Flutter extensions
- **Platform tools**:
  - **Android**: Android Studio with Android SDK
  - **iOS**: Xcode (macOS only)
- **Git** for version control

Verify your setup:
```bash
flutter doctor
```

## Getting Started

1. **Fork and clone**
   ```bash
   git clone https://github.com/YOUR_USERNAME/Evenly.git
   cd Evenly
   git remote add upstream https://github.com/sravan1946/Evenly.git
   ```

2. **Install dependencies**
   ```bash
   flutter pub get
   ```

## Running the App

### Check available devices
```bash
flutter devices
```

### Run on Android
```bash
flutter run -d android
```

### Run on iOS (macOS only)
```bash
flutter run -d ios
```

### Release mode
```bash
flutter run --release
```

## Debugging

### VS Code
- Press `F5` to start debugging
- Set breakpoints by clicking in the gutter
- Use the Debug Console to inspect variables

### Android Studio/IntelliJ
- Click "Run" or press `Shift+F10`
- Set breakpoints and use the debugger panel

### Command Line
- `flutter run` - Run in debug mode
- `r` - Hot reload (while app is running)
- `R` - Hot restart
- `q` - Quit

### Flutter DevTools
```bash
flutter pub global activate devtools
flutter pub global run devtools
```
Or launch from your IDE's debug panel.

## Development Workflow

### 1. Create a Branch
```bash
git checkout main
git pull upstream main
git checkout -b feature/your-feature-name
```

**Branch naming**:
- `feature/` - new features
- `fix/` - bug fixes
- `docs/` - documentation
- `refactor/` - code refactoring

### 2. Make Your Changes
- Write clean, readable code
- Follow existing code style
- Add comments for complex logic
- Update tests if needed

### 3. Test Your Changes
```bash
# Run all tests
flutter test

# Run with coverage
flutter test --coverage
```

### 4. Format and Analyze
```bash
flutter format .
flutter analyze
```

The project uses `flutter_lints` - make sure `flutter analyze` passes with no errors.

### 5. Commit
```bash
git add .
git commit -m "Add feature: description"
```

**Commit guidelines**:
- Use imperative mood ("Add feature" not "Added feature")
- Keep first line under 50 characters
- Reference issues: "Fix #123"

### 6. Keep Branch Updated
```bash
git fetch upstream
git rebase upstream/main
```

### 7. Push and Create PR
```bash
git push -u origin feature/your-feature-name
```

Then open a Pull Request on GitHub. The PR template will guide you through the details.

## Making a Pull Request

### Before Creating PR
- ✅ All tests pass (`flutter test`)
- ✅ Code formatted (`flutter format .`)
- ✅ No analysis issues (`flutter analyze`)
- ✅ Branch is up to date with `main`

### PR Checklist
- Fill out the PR template completely
- Include screenshots for UI changes
- Test on both Android and iOS (if applicable)
- Link related issues

### After PR is Merged
```bash
git checkout main
git pull upstream main
git branch -d feature/your-feature-name
```

## Code Style

Follow [Effective Dart](https://dart.dev/guides/language/effective-dart):

- **Formatting**: Always run `flutter format .` before committing
- **Naming**: 
  - Classes: `PascalCase`
  - Variables/functions: `camelCase`
  - Private: `_leadingUnderscore`
- **Documentation**: Use dartdoc comments (`///`) for public APIs
- **Widgets**: Keep them small and focused, use `const` where possible

The project uses `flutter_lints` - see `analysis_options.yaml` for lint rules.

## Testing

```bash
# Run all tests
flutter test

# Run specific test
flutter test test/widget_test.dart

# Run with coverage
flutter test --coverage
```

Write tests for:
- Business logic (unit tests)
- UI components (widget tests)
- User flows (integration tests)

## Getting Help

- Check [GitHub Issues](https://github.com/sravan1946/Evenly/issues)
- Use GitHub Discussions for questions
- [Flutter Documentation](https://flutter.dev/docs)

---

Thank you for contributing to Evenly! 🎉
