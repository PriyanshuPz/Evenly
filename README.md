# Evenly

Evenly is a simple app for splitting bills with friends. Scan the receipt, assign items, and move on.

## Features

- 📸 Scan receipts
- 👥 Split bills with friends
- 🔒 Offline-first and privacy-focused
- 📱 Cross-platform (Android, iOS)

## Getting Started

### Prerequisites

- Flutter SDK (3.9.2 or compatible)
- Dart SDK (comes with Flutter)
- IDE: VS Code, Android Studio, or IntelliJ IDEA with Flutter extensions

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/sravan1946/Evenly.git
   cd Evenly
   ```

2. Install dependencies:
   ```bash
   flutter pub get
   ```

3. Verify your setup:
   ```bash
   flutter doctor
   ```

### Running the App

```bash
# Run on connected device/emulator
flutter run

# Run on specific platform
flutter run -d android    # Android
flutter run -d ios        # iOS (macOS only)
```

### Debugging

- **VS Code**: Press `F5` to start debugging
- **Android Studio**: Click the "Run" button or press `Shift+F10`
- **Command Line**: Use `flutter run` and press `r` for hot reload, `R` for hot restart

For more detailed debugging instructions, see [CONTRIBUTING.md](CONTRIBUTING.md#debugging).

## Contributing

We welcome contributions! Please read our [Contributing Guide](CONTRIBUTING.md) for details on:

- How to set up your development environment
- How to run and debug the app
- Our development workflow
- How to make a pull request
- Code style guidelines
- Testing requirements

### Quick Start for Contributors

1. Fork the repository
2. Create a branch: `git checkout -b feature/your-feature-name`
3. Make your changes
4. Run tests: `flutter test`
5. Format code: `flutter format .`
6. Analyze code: `flutter analyze`
7. Commit your changes: `git commit -m "Add feature: description"`
8. Push to your fork: `git push origin feature/your-feature-name`
9. Open a Pull Request

For the complete workflow, see [CONTRIBUTING.md](CONTRIBUTING.md).

## Development

### Running Tests

```bash
# Run all tests
flutter test

# Run with coverage
flutter test --coverage
```

### Code Formatting

```bash
# Format all code
flutter format .

# Analyze code
flutter analyze
```

## License

See [LICENSE](LICENSE) file for details.
