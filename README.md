# Rusty2048 🎮

A modern implementation of the 2048 game written in Rust, supporting multi-platform deployment.

## ✨ Features

- **High Performance**: Built with Rust, zero-cost abstractions
- **Cross-Platform**: Supports CLI, Web, and Desktop versions
- **Modern UI**: Smooth animations and beautiful interfaces
- **Configurable**: Customizable board size, target score, and more
- **Replay System**: Record and replay game sessions
- **AI Mode**: Simple AI algorithm demonstration
- **Theme System**: Multiple color schemes

## 🏗️ Project Architecture

```
rusty2048/
├── core/           # Core game logic library
├── cli/            # Command-line version (TUI)
├── web/            # Web version (WASM)
├── desktop/        # Desktop version (Tauri)
└── shared/         # Shared components
```

## 🚀 Quick Start

### Build and Run CLI Version

```bash
# Build the entire project
cargo build

# Run CLI version
cargo run -p rusty2048-cli
```

### Controls

- **Arrow Keys** or **WASD**: Move tiles
- **R**: Restart game
- **U**: Undo last move
- **Q** or **ESC**: Quit game

### Game Features

- **Real-time Statistics**: Display current score, best score, moves, and game duration
- **Game Over Handling**: Show detailed statistics when no moves are possible
- **Victory Notification**: Display victory message when reaching 2048
- **Score Animation**: Score flashes when tiles merge
- **Sound Feedback**: Play bell sound when score increases

## 🛠️ Development

### Requirements

- Rust 1.70+
- Cargo

### Project Structure

- `core/`: Core game logic, including board, moves, scoring, etc.
- `cli/`: Command-line interface using ratatui and crossterm
- `web/`: Web version using wasm-bindgen
- `desktop/`: Desktop version using Tauri

### Testing

```bash
# Run all tests
cargo test

# Run benchmarks
cargo bench

# Run property tests
cargo test --features proptest
```

## 📦 Build Targets

### CLI Version
```bash
cargo build --release -p rusty2048-cli
```

### Web Version (Planned)
```bash
cargo build --target wasm32-unknown-unknown -p rusty2048-web
wasm-pack build web/
```

### Desktop Version (Planned)
```bash
cargo tauri build -p rusty2048-desktop
```

## 🎯 Development Roadmap

- [x] Core game logic
- [x] CLI version basic functionality
- [x] CLI version game over handling
- [x] CLI version score statistics and animations
- [ ] CLI version theme system
- [ ] Web version (WASM)
- [ ] Desktop version (Tauri)
- [ ] Replay system
- [ ] AI mode
- [ ] Statistics charts
- [ ] Multi-language support

## 🤝 Contributing

Contributions are welcome! Please see [CONTRIBUTING.md](CONTRIBUTING.md) for details.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

**Enjoy the game!** 🎉
