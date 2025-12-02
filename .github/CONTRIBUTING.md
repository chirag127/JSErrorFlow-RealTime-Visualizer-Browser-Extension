# 🤝 Contributing to JSErrorFlow-Real-Time-Visualizer-Browser-Extension

Thank you for considering contributing to the JSErrorFlow-Real-Time-Visualizer-Browser-Extension project! We welcome any contributions that help improve the project's quality, functionality, and reach.

## 🌟 Project Philosophy & Standards

This project adheres to the Apex Technical Authority's principles of **Zero-Defect, High-Velocity, Future-Proof** development. All contributions should reflect these standards, aiming for professional-grade code, comprehensive testing, and clear documentation.

## 🚀 Getting Started

### 1. Prerequisites

*   **Git:** Installed and configured. ([Git Documentation](https://git-scm.com/doc))
*   **Node.js:** Latest LTS version recommended. ([Node.js Website](https://nodejs.org/))
*   **npm/Yarn/pnpm:** Package manager. We recommend using `pnpm` for efficiency.
*   **Extension Development Environment:** Familiarity with browser extension development for Chrome/Firefox.

### 2. Setting Up Your Development Environment

To get started, clone the repository and install dependencies:

bash
# Clone the repository
git clone git@github.com:chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension.git
cd JSErrorFlow-Real-Time-Visualizer-Browser-Extension

# Install dependencies (using pnpm is recommended)
pnpm install


### 3. Running the Extension Locally

Our build process is managed by Vite. You can start a development server to see your changes in real-time:

bash
# Start the development server
pnpm dev


This command will typically build the extension and prepare it for loading into your browser. Refer to the `README.md` for specific instructions on loading the development build into your browser (e.g., Chrome's `chrome://extensions` page).

## 📈 Contribution Workflow

We follow a standard GitHub pull request workflow:

1.  **Fork the Repository:** Create your own fork of `chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension`.
2.  **Create a Branch:** Make a new branch for your feature or bug fix (e.g., `feat/add-new-feature`, `fix/resolve-specific-bug`). Use clear and descriptive branch names.
    bash
    git checkout -b your-branch-name
    
3.  **Implement Changes:** Make your desired changes. Ensure your code adheres to the project's coding standards and architectural principles (see AGENTS.md for directives).
4.  **Test Your Changes:** Write unit or integration tests for new functionality and ensure all existing tests pass.
    bash
    pnpm test
    
5.  **Lint and Format:** Ensure your code is clean and adheres to our linting rules.
    bash
    pnpm lint
    pnpm format
    
6.  **Commit Your Changes:** Commit your changes with clear, concise, and conventional commit messages.
    bash
    git commit -m "feat: Add descriptive error messages"
    
7.  **Push to Your Fork:** Push your branch to your forked repository.
    bash
    git push origin your-branch-name
    
8.  **Open a Pull Request:** Submit a pull request from your branch to the `main` branch of the `chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension` repository.

## 🐛 Reporting Bugs

If you find a bug, please submit an issue using the **Bug Report** template. Provide as much detail as possible, including:

*   A clear and concise description of the bug.
*   Steps to reproduce the bug.
*   Expected behavior vs. actual behavior.
*   Browser version and operating system.
*   Screenshots or screen recordings, if applicable.
*   Any relevant error messages from the console.

## ✨ Suggesting Enhancements

We welcome suggestions for new features or improvements. Please submit an issue using the **Feature Request** template. Describe the enhancement and explain why it would be beneficial.

## 📄 Code of Conduct

This project adheres to a Contributor Covenant Code of Conduct. By participating, you are expected to uphold this code. Please refer to the [CODE_OF_CONDUCT.md](https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension/blob/main/CODE_OF_CONDUCT.md) for more details.

## 🤝 Licensing

By contributing to this project, you agree that your contributions will be licensed under the **CC BY-NC 4.0 License** ([LICENSE](https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension/blob/main/LICENSE)).

## 🤖 AI Agent Directives

This project is managed with strict adherence to the AI Agent Directives as defined in [AGENTS.md](https://github.com/chirag127/JSErrorFlow-Real-Time-Visualizer-Browser-Extension/blob/main/AGENTS.md). Ensure your contributions align with the specified architecture, tooling, and quality standards.

---