# 📘 JavaScript Error Visualizer

![JavaScript Error Visualizer Logo](extension/assets/icons/icon128.png)

## ✨ Description

JavaScript Error Visualizer is a browser extension that visually highlights DOM elements associated with JavaScript errors, making debugging faster and more intuitive. It provides immediate visual feedback directly on the webpage, pinpointing the exact elements where errors are occurring.

## 🚀 Live Demo

[View the JavaScript Error Visualizer Website](https://chirag127.github.io/JavaScript-Error-Visualizer-browser-extension/)

## 🛠️ Tech Stack / Tools Used

-   JavaScript (ES6+)
-   Chrome Extension API
-   Source Map library for stack trace translation
-   Webpack for bundling
-   Babel for transpilation
-   Jest for testing
-   HTML5 & CSS3 for UI

## 📦 Installation Instructions

### From Web Store

_Coming soon_

### Manual Installation

1. Clone this repository:

    ```
    git clone https://github.com/chirag127/JavaScript-Error-Visualizer-browser-extension.git
    ```

2. Install dependencies:

    ```
    npm install
    ```

3. Build the extension:

    ```
    npm run build
    ```

4. Load the extension in your browser:
    - Chrome/Edge: Go to `chrome://extensions/`, enable Developer mode, click "Load unpacked", and select the `dist` folder.
    - Firefox: Go to `about:debugging#/runtime/this-firefox`, click "Load Temporary Add-on", and select any file in the `dist` folder.

## Project Structure

```
/
├── extension/
│   ├── manifest.json          # Extension manifest
│   ├── assets/                # Static assets
│   │   ├── icons/             # Extension icons
│   │   ├── css/               # Stylesheets
│   ├── html/                  # HTML files
│   │   ├── popup.html         # Extension popup
│   │   ├── settings.html      # Settings page
│   ├── js/                    # JavaScript files
│   │   ├── modules/           # Core modules
│   │   │   ├── errorCapturer.js    # Error capturing
│   │   │   ├── sourceMapper.js     # Source map handling
│   │   │   ├── elementIdentifier.js # DOM element identification
│   │   │   ├── highlighter.js      # Visual highlighting
│   │   │   ├── settingsManager.js  # Settings management
│   │   │   ├── utils.js            # Utility functions
│   │   ├── background.js      # Background script
│   │   ├── contentScript.js   # Content script
│   │   ├── popup.js           # Popup script
│   │   ├── settings.js        # Settings script
├── test/                      # Tests
├── docs/                      # Documentation
├── index.html                 # Landing page
├── privacy-policy.html        # Privacy policy
├── webpack.config.js          # Webpack configuration
├── package.json               # Project configuration
```

## 🔧 Usage

1. **Enable/Disable**: Click the extension icon and use the toggle switch to enable or disable the extension.

2. **View Errors**: When an error occurs, the associated DOM element will be highlighted on the page. Click the extension icon to see a list of all errors.

3. **Error Details**: Click on an error in the list to see detailed information, including the full stack trace.

4. **Navigate to Elements**: Click on the element links in the error details to scroll to and flash the highlighted element on the page.

5. **Clear Errors**: Use the "Clear All" button to remove all error highlights and reset the error list.

6. **Settings**: Click the "Settings" button to access the extension settings, where you can customize the highlight style, domain settings, and more.

## 🧪 Features

-   **Visual Error Highlighting**: Automatically highlights DOM elements associated with JavaScript errors directly on the webpage.
-   **Comprehensive Error Capture**: Captures uncaught exceptions, unhandled promise rejections, and optionally console.error messages.
-   **Source Map Integration**: Translates stack traces from minified/transpiled code back to the original source code.
-   **Detailed Error Information**: Provides tooltips with error messages and source information when hovering over highlighted elements.
-   **Error Management Panel**: Lists all captured errors with filtering and search capabilities.
-   **Customizable Highlighting**: Allows users to customize the highlight style (color, border style, opacity).
-   **Domain-specific Settings**: Enable/disable the extension for specific domains.

## 📸 Screenshots

_Coming soon_

## 🙌 Contributing

Contributions are welcome! Here's how you can contribute:

1. Fork the repository
2. Create a feature branch: `git checkout -b feature/your-feature-name`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin feature/your-feature-name`
5. Open a pull request

Please make sure to update tests as appropriate and follow the code style of the project.

## 🪪 License

MIT
