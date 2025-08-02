# MySAI Assistant

A powerful, cross-platform AI assistant app built with Flutter that provides intelligent chat experiences across multiple content types.

## 🚀 Features

### 🤖 Multiple AI Assistants

-   **Text Assistant**: General-purpose AI chat for questions, writing, and conversations
-   **Image Assistant**: AI-powered image analysis and description
-   **PDF Assistant**: Document analysis and question-answering from PDF files

### 💬 Smart Chat Interface

-   Modern, intuitive chat UI with Material 3 design
-   Persistent chat history with local storage
-   Real-time message delivery
-   Support for multiple concurrent conversations

### 🔧 Core Capabilities

-   **File Upload**: Support for PDF documents and images
-   **Secure Storage**: Encrypted storage for API keys and sensitive data
-   **Cross-Platform**: Runs on iOS, Android, Web, and Windows
-   **Offline Storage**: Local chat history with Hive database
-   **Custom Theming**: Beautiful dark theme with gradient backgrounds

## 📱 Screenshots

_Chat with different AI assistants for various content types_

## 🛠️ Tech Stack

-   **Framework**: Flutter (Dart)
-   **AI Integration**: Google Gemini API
-   **State Management**: Riverpod
-   **Local Database**: Hive
-   **Navigation**: GoRouter
-   **UI Components**: Material 3
-   **Animations**: Lottie
-   **File Handling**: File Picker, Image Picker
-   **PDF Processing**: Syncfusion PDF Viewer

## 📋 Prerequisites

-   Flutter SDK (>=3.1.3)
-   Dart SDK
-   Google Gemini API Key
-   iOS/Android development environment (for mobile builds)

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/vonuyvicoo/flutter-ai-nda-base-app
cd flutter-ai-nda-base-app
```

### 2. Install Dependencies

```bash
flutter pub get
```

### 3. Generate Code

```bash
flutter packages pub run build_runner build
```

### 4. Configure API Keys

1. Launch the app
2. On first run, you'll be prompted to enter your Google Gemini API key
3. Get your API key from [Google AI Studio](https://makersuite.google.com/app/apikey)

### 5. Run the App

```bash
# For development
flutter run

# For specific platforms
flutter run -d ios
flutter run -d android
flutter run -d web
flutter run -d windows
```

## 🏗️ Build for Production

### Android

```bash
flutter build apk --release
# or for app bundle
flutter build appbundle --release
```

### iOS

```bash
flutter build ios --release
```

### Web

```bash
flutter build web --release
```

### Windows

```bash
flutter build windows --release
```

## 📂 Project Structure

```
lib/
├── core/
│   ├── app/           # App configuration and theming
│   ├── config/        # Constants and configuration
│   ├── extension/     # Dart extensions
│   ├── navigation/    # Routing and navigation
│   └── util/          # Utility functions
├── feature/
│   ├── chat/          # Chat interface and logic
│   ├── gemini/        # AI integration
│   ├── hive/          # Local database models
│   ├── home/          # Home screen with assistant selection
│   └── welcome/       # Onboarding and setup
└── main.dart          # App entry point
```

## 🎨 Customization

### Themes

The app uses a custom dark theme with vibrant accent colors. You can modify the theme in `lib/core/app/style.dart`:

```dart
const _primary = Color(0xFFFF6B35);     // Primary orange
const _secondary = Color(0xFF9B59B6);   // Secondary purple
const _tertiary = Color(0xFFFFB347);    // Tertiary peach
```

### AI Models

The app currently uses Google Gemini Pro. You can extend support for other AI providers by implementing the `BaseGeminiRepository` interface.

## 🔐 Security

-   API keys are stored securely using `flutter_secure_storage`
-   Local chat data is stored using Hive with encryption support
-   No chat data is transmitted to external servers except AI API calls

## 🐛 Troubleshooting

### Common Issues

**Build Errors on iOS**

-   Ensure you have the latest Xcode and iOS SDK
-   Run `flutter clean` and `flutter pub get`
-   Check iOS deployment target compatibility

**Android Build Issues**

-   Verify Android SDK and build tools are up to date
-   Check `android/app/build.gradle` for version conflicts

**API Key Issues**

-   Verify your Gemini API key is valid
-   Check API quotas and billing in Google Cloud Console
-   Ensure the API key has proper permissions

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

-   Google Gemini AI for powering the chat capabilities
-   Flutter team for the amazing framework
-   Syncfusion for PDF processing components
-   Lottie for smooth animations

## 📞 Support

For support, email von@sanghaya.org or create an issue on GitHub.

---

**MySAI Assistant** - Your intelligent companion for text, images, and documents.
