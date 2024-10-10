# Smart Translate Lints

[![Pub Version](https://img.shields.io/pub/v/smart_translate_lints)](https://pub.dev/packages/smart_translate_lints)
[![Dart SDK](https://img.shields.io/badge/Dart%20SDK-%20%3E%3D2.12.0%20%3C3.0.0-blue)](https://dart.dev)

## Introduction

Smart Translate Lints is a custom linting plugin for Flutter that helps catch missing translation strings in your code. It ensures that all strings are localized using locale key variables, enhancing the accessibility and internationalization of your applications.

## Installation

To install Smart Translate Lints, add it as a dependency in your `pubspec.yaml` file:

```yaml
dev_dependencies:
  custom_lint: ^latest_version
  smart_translate_lints: ^1.0.0
```

Then, run `flutter pub get` to fetch the package.

## Configuration

To use Smart Translate Lints, you need to include it in your `analysis_options.yaml` file:

```yaml

analyzer:
  plugins:
    - custom_lint

custom_lint:
  rules:
    - smart_translate_lint_role: true # for enabled or false for disabled
```

This will enable the linting rules provided by Smart Translate Lints in your Flutter project.

## Usage

Once installed and configured, Smart Translate Lints will automatically check your code for missing translation strings. If a string is not localized using a locale key variable, the linter will raise a warning.

## Conclusion

Smart Translate Lints is an essential tool for maintaining high-quality, accessible code in multilingual Flutter applications. By catching and warning about missing translations, it helps ensure that your app can reach a global audience.
