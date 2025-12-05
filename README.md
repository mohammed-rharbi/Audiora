# 🎵 Audiora

A modern, sleek music streaming and player application built with **React Native** and **Expo**. Discover, play, and manage your favorite tracks with an intuitive interface designed for music lovers.

---

## ✨ Features

### Core Functionality
- **🎶 Music Playback** - High-quality audio streaming with play, pause, skip, and seek controls
- **🔍 Search & Discover** - Find your favorite songs, artists, and albums instantly
- **📋 Playlist Management** - Create, edit, and organize your custom playlists
- **❤️ Favorites** - Mark and save your favorite tracks for quick access
- **🔄 Queue Management** - Manage the playback queue with drag-and-drop reordering

### Advanced Features
- **🌙 Dark Mode** - Beautiful dark theme for comfortable listening in any lighting
- **🔊 Volume Control** - Fine-grained audio level adjustments
- **⏱️ Progress Bar** - Visual playback progress with seek functionality
- **🎨 Modern UI** - Clean, responsive design optimized for mobile devices
- **🚀 Fast Performance** - Smooth animations and instant app responsiveness

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| **Framework** | React Native |
| **Build Tool** | Expo |
| **Language** | JavaScript / TypeScript |
| **Audio Playback** | Expo Audio API |
| **Navigation** | Expo Router |
| **Styling** | Tailwind CSS (NativeWind) |
| **State Management** | React Hooks / Context API |
| **Platform Support** | iOS, Android, Web |

---

## 📱 Installation & Setup

### Prerequisites
- **Node.js** v18+ and npm/yarn
- **Expo CLI**: `npm install -g expo-cli`
- **Android Studio** (for Android development) or **Xcode** (for iOS)
- **Expo Go app** on your mobile device (for testing)

### Quick Start

1. **Clone the repository**
   git clone https://github.com/your-username/Audiora.git
   cd Audiora

2. **Install dependencies**
   npm install
   # or
   yarn install

3. **Start the development server**
   npx expo start

4. **Run on your device**
   - **Android**: Press `a` to open in Android Emulator, or scan QR code with Expo Go app
   - **iOS**: Press `i` to open in iOS Simulator, or scan QR code with iPhone Camera app
   - **Web**: Press `w` to open in your browser

### Environment Variables

Create a `.env` file in the project root (optional for future API integrations):

EXPO_PUBLIC_API_URL=https://api.example.com
EXPO_PUBLIC_API_KEY=your_api_key_here

---

## 🎯 Project Structure

Audiora/
├── app/                      # Expo Router (File-based routing)
│   ├── _layout.tsx          # Root layout with navigation
│   ├── (tabs)/              # Tabbed navigation screens
│   │   ├── index.tsx        # Home / Now Playing
│   │   ├── search.tsx       # Search & Discover
│   │   ├── playlists.tsx    # Playlist Management
│   │   └── profile.tsx      # User Profile
│   ├── player/              # Player detail view
│   └── +not-found.tsx       # 404 fallback
├── components/              # Reusable UI components
│   ├── PlayerControls.tsx   # Play/Pause/Skip buttons
│   ├── TrackCard.tsx        # Individual track display
│   ├── PlaylistItem.tsx     # Playlist item component
│   └── ProgressBar.tsx      # Audio progress visualization
├── services/                # Business logic & APIs
│   ├── audioService.ts      # Expo Audio wrapper
│   ├── playlistService.ts   # Playlist management
│   └── searchService.ts     # Search functionality
├── hooks/                   # Custom React Hooks
│   ├── usePlayer.ts         # Player state & controls
│   ├── usePlaylists.ts      # Playlist operations
│   └── useSearch.ts         # Search logic
├── context/                 # Context API for global state
│   ├── AudioContext.tsx     # Audio playback context
│   └── AppContext.tsx       # App-wide settings
├── types/                   # TypeScript type definitions
│   ├── audio.ts             # Audio-related types
│   └── playlist.ts          # Playlist types
├── styles/                  # Global styles & theme
│   └── theme.ts             # Color palette & design tokens
├── assets/                  # Images, icons, fonts
│   ├── icons/
│   └── images/
├── app.json                 # Expo configuration
├── eas.json                 # EAS Build configuration
└── package.json             # Project dependencies

---

## 🚀 Development Workflow

### Running Tests
npm run test
# or with coverage
npm run test:coverage

### Building for Production

#### Android APK
eas build --platform android

#### iOS App
eas build --platform ios

#### Web Build
expo export --platform web

### Debugging
- **React DevTools**: Press `j` in Expo CLI menu
- **Network Inspector**: Built-in Expo DevTools
- **Console Logs**: Visible in terminal running `npx expo start`

---

## 📚 Key Dependencies

{
  "react": "^18.3.0",
  "react-native": "^0.81.5",
  "expo": "^54.0.26",
  "expo-router": "^3.x",
  "expo-audio": "^16.x",
  "nativewind": "^2.x",
  "react-native-reanimated": "^3.x",
  "zustand": "^4.x"
}

*See `package.json` for the complete dependency list.*

---

## 🎨 Design Philosophy

Audiora prioritizes **user experience** and **performance**:

- **Minimalist UI** - Focus on music, not clutter
- **Smooth Animations** - Native performance with React Native Reanimated
- **Responsive Design** - Adapts seamlessly from small phones to tablets
- **Accessibility** - WCAG compliance with proper contrast ratios and focus states
- **Dark Mode First** - Reduces eye strain during extended listening sessions

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork the repository**
   git clone https://github.com/your-username/Audiora.git

2. **Create a feature branch**
   git checkout -b feature/your-feature-name

3. **Make your changes** and commit with clear messages
   git commit -m "feat: add lyrics display feature"

4. **Push to your fork**
   git push origin feature/your-feature-name

5. **Open a Pull Request** with a detailed description

### Coding Guidelines
- Use **TypeScript** for type safety
- Follow **ESLint** and **Prettier** rules
- Write **unit tests** for new features (minimum 80% coverage)
- Follow the existing **folder structure** and naming conventions
- Document complex functions with **JSDoc comments**

---

## 🐛 Known Issues & Roadmap

### Current Limitations
- Web version has limited audio format support
- Some native features unavailable on web platform
- Background playback requires specific configuration on Android

### Upcoming Features (v2.0)
- 🎤 Lyrics synchronization with playback
- 🎧 Equalizer controls
- 🌐 Cloud sync across devices
- 🤖 AI-powered playlist recommendations
- 🎙️ Podcast support
- 📻 Radio mode

---

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](./LICENSE) file for details.

---

## 📞 Support & Contact

Have questions or need help?

- **Issues**: [GitHub Issues](https://github.com/your-username/Audiora/issues)
- **Email**: support@audiora.app
- **Discord**: [Join our community](#)
- **Twitter**: [@AudioraApp](#)

---

## 🙏 Acknowledgments

- [Expo Documentation](https://docs.expo.dev) for excellent React Native tooling
- [React Native Community](https://github.com/react-native-community) for invaluable libraries
- All contributors who have helped shape Audiora

---

## 📊 Project Stats

![GitHub Stars](https://img.shields.io/github/stars/your-username/Audiora?style=flat-square)
![GitHub Forks](https://img.shields.io/github/forks/your-username/Audiora?style=flat-square)
![GitHub Issues](https://img.shields.io/github/issues/your-username/Audiora?style=flat-square)
![License](https://img.shields.io/badge/license-MIT-blue?style=flat-square)

---

**Made with 🎵 by the Audiora Team**

*Last Updated: December 2025*
