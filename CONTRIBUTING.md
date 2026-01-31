# Contributing to FilterDNS Client

Thank you for your interest in contributing to FilterDNS Client! This document provides guidelines and instructions for contributing.

## Getting Started

### Prerequisites

- Go 1.22+
- Node.js 18+
- Wails v2 (`go install github.com/wailsapp/wails/v2/cmd/wails@latest`)

**Linux:**
```bash
sudo apt install libgtk-3-dev libwebkit2gtk-4.1-dev
```

**macOS:**
- Xcode Command Line Tools

**Windows:**
- WebView2 Runtime (usually pre-installed on Windows 10/11)

### Development Setup

1. Fork and clone the repository:
   ```bash
   git clone https://github.com/YOUR_USERNAME/filterdns-client.git
   cd filterdns-client
   ```

2. Install dependencies:
   ```bash
   make install-deps
   ```

3. Run in development mode:
   ```bash
   make dev
   ```

## Making Changes

### Code Style

- **Go**: Follow standard Go conventions. Use `go fmt` and `go vet`:
  ```bash
  go fmt ./...
  go vet ./...
  ```

- **TypeScript/Svelte**: We use Prettier and ESLint:
  ```bash
  cd frontend && npm run lint && npm run format
  ```

### Building

```bash
# Build for current platform
make build

# Build for all platforms
make build-all
```

## Pull Request Process

1. **Create a branch** for your changes:
   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Make your changes** and commit with clear messages:
   ```bash
   git commit -m "Add feature: description of what it does"
   ```

3. **Test your changes** on your platform

4. **Push your branch** and create a pull request:
   ```bash
   git push origin feature/your-feature-name
   ```

5. **Describe your changes** in the PR description:
   - What does this PR do?
   - Why is this change needed?
   - How was it tested?
   - Which platforms were tested?

## Reporting Issues

When reporting bugs, please include:

- Your environment (OS, Go version, Wails version)
- Steps to reproduce the issue
- Expected vs actual behavior
- Relevant logs or error messages

## Questions?

Feel free to open an issue for questions or discussions about the project.
