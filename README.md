# Keyword Colorizer

**Keyword Colorizer** gives you full control over your syntax highlighting. Easily assign custom colors and font weights to specific keywords, variables, or patterns across your workspace.

Whether you want `return` statements to be bright red, or you need `TODO` comments to stand out in neon green, this extension lets you customize it directly from the VS Code Settings UI.

## Features

*   **Custom Colors:** Assign any hex color to any word.
*   **Bold Styling:** Toggle bold font weight for extra emphasis.
*   **Live Updates:** Colors update instantly as you type or change settings.
<!-- *   **Settings UI Support:** configure everything via dropdowns and color pickers—no JSON editing required. -->
*   **Language Agnostic:** Works in TypeScript, Python, C++, Java, Text, and more.

## How to Use
<!-- 
### Via Settings UI (Recommended)
1. Open VS Code Settings (`Ctrl + ,` or `Cmd + ,`).
2. Search for **Keyword Colorizer**.
3. Under **Keyword Colorizer: Styles**, click **Add Item**.
4. Enter the **Keyword** (e.g., `function`, `return`, `get`).
5. Pick a **Color** (hex code).
6. Check **Is Bold** if desired. -->

### Via settings.json
You can also configure it manually in your `.vscode/settings.json` or User Settings
```json
  "keywordColorizer.styles": [
    // ===== Current defaults =====

    // ===== Declarations =====
    { "keyword": "function", "color": "#4ECDC4", "isBold": false },
    { "keyword": "class", "color": "#82AAFF", "isBold": false },
    { "keyword": "interface", "color": "#C678DD", "isBold": false },
    { "keyword": "type", "color": "#D19A66", "isBold": false },
    { "keyword": "enum", "color": "#98C379", "isBold": false },
    { "keyword": "struct", "color": "#E06C75", "isBold": false },
    { "keyword": "namespace", "color": "#E5C07B", "isBold": false },
    { "keyword": "module", "color": "#7FDBCA", "isBold": false },
    { "keyword": "new", "color": "#FF6F91", "isBold": false },
    { "keyword": "constructor", "color": "#B39DDB", "isBold": false },
    { "keyword": "get", "color": "#80CBC4", "isBold": false },
    { "keyword": "set", "color": "#FFB74D", "isBold": false },
    { "keyword": "extends", "color": "#A5D6A7", "isBold": false },
    { "keyword": "implements", "color": "#F48FB1", "isBold": false },

    // ===== Control Flow / Exit =====
    { "keyword": "return", "color": "#e8f12dff", "isBold": false },
    { "keyword": "throw", "color": "#D32F2F", "isBold": false },
    { "keyword": "break", "color": "#e7f12dd8", "isBold": false },
    { "keyword": "continue", "color": "#cdd538ff", "isBold": false },
    { "keyword": "yield", "color": "#c4cd1bff", "isBold": false },
    { "keyword": "debugger", "color": "#880E4F", "isBold": false },
    { "keyword": "goto", "color": "#6A1B9A", "isBold": false },
    { "keyword": "delete", "color": "#4A148C", "isBold": false },

    // ===== Conditionals / Loops =====
    { "keyword": "if", "color": "#9575CD", "isBold": false },
    { "keyword": "else", "color": "#7986CB", "isBold": false },
    { "keyword": "switch", "color": "#5C6BC0", "isBold": false },
    { "keyword": "case", "color": "#3F51B5", "isBold": false },
    { "keyword": "default", "color": "#3949AB", "isBold": false },
    { "keyword": "for", "color": "#303F9F", "isBold": false },
    { "keyword": "while", "color": "#283593", "isBold": false },
    { "keyword": "do", "color": "#1A237E", "isBold": false },
    { "keyword": "with", "color": "#64B5F6", "isBold": false },
    { "keyword": "typeof", "color": "#42A5F5", "isBold": false },
    { "keyword": "in", "color": "#2196F3", "isBold": false },
    { "keyword": "of", "color": "#1E88E5", "isBold": false },

    // ===== Variable Modifiers =====
    { "keyword": "const", "color": "#26C6DA", "isBold": false },
    { "keyword": "let", "color": "#00BCD4", "isBold": false },
    { "keyword": "var", "color": "#00ACC1", "isBold": false },
    { "keyword": "static", "color": "#0097A7", "isBold": false },
    { "keyword": "final", "color": "#00838F", "isBold": false },
    { "keyword": "readonly", "color": "#006064", "isBold": false },
    { "keyword": "volatile", "color": "#4DD0E1", "isBold": false },
    { "keyword": "instanceof", "color": "#80DEEA", "isBold": false },

    // ===== Imports / Access =====
    { "keyword": "import", "color": "#FFD54F", "isBold": false },
    { "keyword": "export", "color": "#FFCA28", "isBold": false },
    { "keyword": "from", "color": "#FFC107", "isBold": false },
    { "keyword": "as", "color": "#FFB300", "isBold": false },
    { "keyword": "package", "color": "#FFA000", "isBold": false },
    { "keyword": "require", "color": "#FF8F00", "isBold": false },
    { "keyword": "using", "color": "#FF6F00", "isBold": false },
    { "keyword": "public", "color": "#C0CA33", "isBold": false },
    { "keyword": "private", "color": "#AFB42B", "isBold": false },
    { "keyword": "protected", "color": "#9E9D24", "isBold": false },
    { "keyword": "abstract", "color": "#827717", "isBold": false },
    { "keyword": "native", "color": "#D4E157", "isBold": false },
    { "keyword": "async", "color": "#AED581", "isBold": false },
    { "keyword": "await", "color": "#81C784", "isBold": false },
    { "keyword": "synchronized", "color": "#66BB6A", "isBold": false },

    // ===== Booleans =====
    { "keyword": "true", "color": "#2E7D32", "isBold": true },
    { "keyword": "false", "color": "#1B5E20", "isBold": true },

    // ===== Types / Nullability =====
    { "keyword": "null", "color": "#FF7043", "isBold": false },
    { "keyword": "undefined", "color": "#FF5722", "isBold": false },
    { "keyword": "void", "color": "#F4511E", "isBold": false },
    { "keyword": "int", "color": "#FB8C00", "isBold": false },
    { "keyword": "float", "color": "#F57C00", "isBold": false },
    { "keyword": "double", "color": "#EF6C00", "isBold": false },
    { "keyword": "char", "color": "#E65100", "isBold": false },
    { "keyword": "byte", "color": "#FF8A65", "isBold": false },
    { "keyword": "short", "color": "#FFAB91", "isBold": false },
    { "keyword": "long", "color": "#FFCCBC", "isBold": false },
    { "keyword": "boolean", "color": "#A1887F", "isBold": false },
    { "keyword": "string", "color": "#8D6E63", "isBold": false },
    { "keyword": "any", "color": "#795548", "isBold": false },
    { "keyword": "unknown", "color": "#6D4C41", "isBold": false },
    { "keyword": "never", "color": "#5D4037", "isBold": false },

    // ===== Special References =====
    { "keyword": "this", "color": "#981ee3ff", "isBold": false },
    { "keyword": "super", "color": "#6956e6ff", "isBold": false },

    // ===== Error Handling (EXCEPTION: shared color) =====
    { "keyword": "try", "color": "#FF5252", "isBold": false },
    { "keyword": "catch", "color": "#FF5252", "isBold": false },
    { "keyword": "finally", "color": "#FF5252", "isBold": false }
  ]