# Kezi ERP Documentation

This repository contains the official documentation for the **Kezi ERP** system. Ideally, it serves as the single source of truth for all user and developer guides, strictly following the **Diátaxis framework**.

## 📚 Documentation Structure

We organize our documentation into four specific categories based on the [Diátaxis framework](https://diataxis.fr/):

1.  **Tutorials** (`tutorials/`): Learning-oriented. Lessons that take the reader by the hand through a series of steps to complete a project of some kind.
2.  **How-To Guides** (`how-to/`): Problem-oriented. Guides that show the reader how to solve a specific problem or complete a specific task.
3.  **Reference** (`reference/`): Information-oriented. Technical descriptions and dry facts (e.g., API specs, field definitions).
4.  **Explanation** (`explanation/`): Understanding-oriented. Discussions that clarify concepts, background, and broad topics.

## 🌍 Languages

The documentation is localized into the following languages:

*   **English** (`en/`) - *Primary*
*   **Central Kurdish** (`ckb/`)
*   **Arabic** (`ar/`)

## ✍️ Contributing

When adding or updating documentation, please adhere to the following rules:

1.  **Diátaxis Compliance**: Ensure your content fits into one of the four distinct quadrants.
2.  **Naming Convention**: Use kebab-case for filenames (e.g., `creating-a-company.md`).
3.  **Language Parity**: Whenever possible, ensure updates are reflected across all supported languages to maintain consistency.
4.  **Format**: All documentation is written in standard Markdown.

## 🚀 Usage

This documentation is consumed by the main Kezi application. Changes pushed to this repository will be reflected in the application's documentation section (typically via a git submodule update or webhook integration).
