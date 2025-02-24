# Dead Code Hunter - VS Code Extension

Dead Code Hunter is a Visual Studio Code extension designed to help developers track and manage unused code in their projects. It integrates with the VS Code diagnostic system to detect **errors**, **warnings**, and **dead code** (unused variables and functions) across your files and lists them in an easy-to-navigate panel. This allows you to quickly identify and clean up unused code, making your project more efficient and maintainable.

## Features

- **Track Errors**: Displays a list of files with errors, making it easier to fix problems in your code.
- **Track Warnings**: Displays a list of files with warnings, helping you address potential issues early.
- **Detect Dead Code**: Identify files that contain **unused functions** or **unused variables** (greyed-out code) and list them separately for review.
- **Grouping and Filtering**: Errors, warnings, and dead code are grouped into separate sections for better organization.
- **Clear List**: A button to clear the list of errors, warnings, and dead code in the panel.
- **Auto-Expanding Sections**: The **Errors** and **Warnings** sections are expanded by default for immediate visibility.

## Installation

### 1. Install from Visual Studio Code Marketplace

You can directly install the Dead Code Hunter extension from the [Visual Studio Code Marketplace](https://marketplace.visualstudio.com/).

1. Open VS Code.
2. Go to the Extensions panel (Ctrl+Shift+X or Cmd+Shift+X).
3. Search for **Dead Code Hunter**.
4. Click **Install**.

### 2. Install Locally (for Development)

If you're working on the extension or want to run it locally:

1. Clone this repository:
   ```bash
   git clone <repository-url>

    Navigate to the extension folder:

  cd <extension-folder>

Install dependencies:

npm install

Compile the extension:

    npm run compile

    Launch the extension in VS Code:
        Press F5 to run the extension in a new VS Code window.

## Usage

    Open your project in VS Code.
    You will see a Dead Code Hunter panel in the Activity Bar.
    The panel will show:
        Errors: Files with errors in your project.
        Warnings: Files with warnings.
        Dead Code: Files that contain unused code (e.g., greyed-out variables or functions).
    You can click on the items in the panel to quickly open and fix the corresponding files.
    Click the "Clear List" button to reset the panel and remove all items.

## Configuration

This extension automatically detects errors, warnings, and dead code based on the diagnostics provided by VS Code. You do not need to configure any settings to start using it, but you can always customize your diagnostics setup via your VS Code settings (e.g., ESLint or other linters).
Contributing

Contributions are welcome! If you'd like to contribute to the extension, please follow these steps:

    Fork the repository.
    Create a new branch (git checkout -b feature/your-feature-name).
    Make your changes and commit them (git commit -am 'Add your feature').
    Push to your branch (git push origin feature/your-feature-name).
    Create a new Pull Request.

## License

This extension is licensed under the MIT License. See the LICENSE file for more information.

## Known Issues:

    Currently, unused code is detected using basic heuristics. It may not catch all instances, depending on the language and tooling setup. Future improvements may integrate with advanced linters like ESLint for more thorough dead code detection.

## Acknowledgements:

    This extension uses VS Code's Diagnostics API to gather error and warning information.
    Unused Code Detection is based on diagnostic messages and may be further refined in the future.
