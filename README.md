# NotAIble

**NotAIble** is a cutting-edge, AI-powered notepad application designed to enhance your productivity and creativity. It leverages the power of AI to provide smart suggestions, making it easier for you to complete your sentences, and supports seamless markdown editing. Built with Rust for a lightning-fast backend and Tauri for a modern desktop experience, NotAIble ensures a smooth and responsive workflow.

## Features

### Core Features
- **AI-Powered Suggestions**:
  - Autocomplete sentences based on context.
  - Powered by locally installed AI models for privacy and performance.
  - Default support for [Ollama](https://www.ollama.com) via `https://localhost:11434/`.
  
- **Markdown Support**:
  - Built-in markdown parser.
  - Syntax highlighting and live preview.
  - Create, edit, and save markdown files directly.

- **Text Summarization**:
  - Summarize large paragraphs into short meaningful sentences.

- **High Performance**:
  - Rust-powered backend ensures low latency and high-speed operations.
  - Efficient handling of large files and complex tasks.

## Installation

### Prerequisites
- **React + Typescript** (for frontend development)
- **Rust** (for backend development)
- **Tauri CLI**
- Local AI model setup (default: [Ollama](https://www.ollama.com))

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/Udhay-Adithya/notaible.git
   cd notaible
   ```

2. Install frontend dependencies:
   ```bash
   yarn install
   ```

3. Build the project:
   ```bash
   yarn run tauri build
   ```

4. Run the app in development mode:
   ```bash
   yarn run tauri dev
   ```

5. Ensure your AI model is running (default: Ollama at `https://localhost:11434/`).

---

## Contribution Guidelines

We welcome contributions to NotAIble! Please read our [Contributing Guide](CONTRIBUTING.md) for details on the code of conduct, bug reports, and pull requests.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

## Feedback

We value your feedback! If you encounter any issues or have suggestions for improvements, please create an issue in the [Issues section](https://github.com/yourusername/notaible/issues).

---

## Project Structure
```plaintext
notaible/
├── public/                # Static assets for the frontend
├── src/                   # Frontend (React + TypeScript) source code
│   ├── components/        # React components
│   ├── pages/             # Page components (if using a routing system)
│   ├── styles/            # CSS/SCSS files
│   ├── utils/             # Utility/helper functions
│   ├── App.tsx            # Main App component
│   ├── main.tsx           # Entry point for React
│   └── index.html         # HTML entry point (referenced in public/index.html)
├── src-tauri/             # Tauri configuration and Rust backend
│   ├── src/               # Rust source code
│   │   ├── main.rs        # Entry point for the Rust backend
│   │   ├── commands.rs    # Custom commands exposed to the frontend
│   │   ├── utils.rs       # Utility functions (optional)
│   │   └── models/        # Models (optional, for organizing data structures)
│   ├── tauri.conf.json    # Tauri configuration file
│   └── Cargo.toml         # Rust dependencies and configuration
├── package.json           # Frontend dependencies and scripts
├── tsconfig.json          # TypeScript configuration
├── vite.config.ts         # Vite configuration (or your bundler's config)
├── .gitignore             # Git ignore file
└── README.md              # Project documentation

```

---

## Acknowledgments

Special thanks to the Tauri and Rust communities for creating amazing tools and frameworks that made NotAIble possible.

