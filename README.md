# Batch Regex Replacer

An Android application for performing batch text replacement operations using regular expressions, inspired by the [aGrep](https://github.com/jiro-aqua/aGrep) Android app.

## Features

- **Regex Pattern Matching**: Use powerful regular expressions to find text patterns
- **Batch Replacement**: Replace all matching patterns with a single operation
- **File Operations**: Support for reading and writing files with regex replacements
- **User-Friendly Interface**: Simple and intuitive UI for entering patterns and text
- **Real-time Feedback**: Immediate feedback on replacement results and error handling

## Requirements

- Android API 21 (Android 5.0) and above
- Android Studio 2022.1 or higher
- Kotlin 1.9.0
- Gradle 8.1.0

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Sado-New/BatchRegexReplacer.git
   cd BatchRegexReplacer
   ```

2. Open the project in Android Studio

3. Build the project:
   ```bash
   ./gradlew build
   ```

4. Run on an emulator or device:
   ```bash
   ./gradlew installDebug
   ```

## Usage

1. Launch the app on your Android device
2. Enter a regex pattern in the "Regex Pattern" field
3. Enter the replacement text in the "Replacement Text" field
4. Enter the text to be replaced in the "Input Text" field
5. Tap the "Replace All" button to perform the replacement
6. View the results in the result area

## Project Structure

```
BatchRegexReplacer/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/example/batchregexreplacer/
│   │   │   │   ├── MainActivity.kt
│   │   │   │   └── RegexReplacer.kt
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   ├── values/
│   │   │   │   └── drawable/
│   │   │   └── AndroidManifest.xml
│   │   └── test/
│   └── build.gradle.kts
├── build.gradle.kts
├── settings.gradle.kts
└── README.md
```

## API Reference

### RegexReplacer Object

#### `replace(text: String, pattern: String, replacement: String): String`
Performs regex replacement on the provided text.

- **Parameters**:
  - `text`: The input text to process
  - `pattern`: The regex pattern to search for
  - `replacement`: The replacement string

- **Returns**: Result message with match count or error information

#### `replaceInFile(filePath: String, pattern: String, replacement: String): Result<String>`
Performs regex replacement on a file's contents.

- **Parameters**:
  - `filePath`: Path to the file to process
  - `pattern`: The regex pattern to search for
  - `replacement`: The replacement string

- **Returns**: Success message with match count or error

## Testing

Run the unit tests with:
```bash
./gradlew test
```

## License

This project is licensed under the Apache License 2.0 - see the LICENSE file for details.

## Acknowledgments

Inspired by [aGrep](https://github.com/jiro-aqua/aGrep) - a grep-like text search tool for Android.

## Contributing

Contributions are welcome! Feel free to submit issues and pull requests.
