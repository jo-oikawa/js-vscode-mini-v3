# Design System Maintenance Instructions

This document provides instructions for keeping the `design-system.html` page up to date as the VS Code Mini prototype evolves.

## Overview

test test test 

The design system page (`design-system.html`) documents the visual language, design tokens, and component patterns used throughout the prototype. It serves as a living reference for:

- **Design tokens** (colors, typography, spacing)
- **UI components** (buttons, tabs, inputs, panels)
- **Icon usage** (Codicon icon set)
- **Art direction decisions**

## When to Update the Design System

Update `design-system.html` whenever you make changes to:

### 1. CSS Custom Properties (Design Tokens)

If you add, modify, or remove CSS variables in `index.html`, update the corresponding section in `design-system.html`:

- **Color tokens** → Update "Color Tokens" section
- **Typography tokens** → Update "Typography" section  
- **Spacing tokens** → Update "Spacing & Layout" section
- **Border radius tokens** → Update "Border Radius" subsection

### 2. Component Styles

If you change the visual appearance of UI components:

- **Buttons** → Update "Buttons & UI Elements" section with new variants/states
- **Tabs** → Update the tabs example
- **Inputs** → Update input field examples
- **Panel headers** → Update panel header examples
- **Activity bar** → Update activity bar item examples
- **Status bar** → Update status bar examples
- **Tree/Explorer items** → Update tree item examples

### 3. Icon Usage

If you introduce new icons from the Codicon set:

- Add them to the relevant icon grid in the "Codicon Icon Set" section
- Group icons by category (UI, Layout, Chat/AI, Navigation, Status)

### 4. New Components

If you add entirely new component patterns:

1. Create a new `<h3>` subsection under the appropriate `<section>`
2. Add a `.component-example` block with:
   - A `.component-label` describing the component
   - A live example of the component
3. Add a `.design-notes` block if there are important usage guidelines

## File Structure

```
design-system.html     # Main design system documentation page
index.html            # Main prototype (source of truth for styles)
assets/
├── codicons/         # Codicon font files
│   ├── codicon.css
│   └── codicon.ttf
└── visual-studio-code-icons/
    ├── vscode.svg    # Product icon (SVG)
    └── vscode.png    # Product icon (PNG)
```

## Checklist for Design System Updates

When making significant visual changes, use this checklist:

- [ ] Update design tokens if CSS variables changed
- [ ] Update component examples if styling changed
- [ ] Add new icons to the icon grid if used
- [ ] Add design notes for non-obvious decisions
- [ ] Update the "Last updated" date in the footer
- [ ] Test the page renders correctly in a browser

## Token Naming Conventions

Follow these naming patterns for new tokens:

| Category | Pattern | Example |
|----------|---------|---------|
| Colors - Background | `--bg-*` | `--bg-elevated` |
| Colors - Foreground | `--fg-*` | `--fg-muted` |
| Colors - Accent | `--accent-*` | `--accent-2` |
| Colors - Semantic | `--danger`, `--success`, `--warning` | |
| Typography | `--fs-*` (size), `--lh-*` (line-height), `--font-*` (family) | `--fs-base` |
| Spacing | `--space-{n}` | `--space-4` |
| Border | `--border`, `--border-*`, `--radius-*` | `--radius-lg` |

## Design Principles

When adding to the design system, maintain these principles:

1. **VS Code Fidelity** - Match VS Code's visual language closely
2. **Dark Theme First** - Primary theme is dark; tokens should work for dark mode
3. **Consistent Spacing** - Use the spacing scale, avoid magic numbers
4. **Semantic Colors** - Use semantic tokens (danger, success) over raw values
5. **Icon Consistency** - Use Codicons exclusively; avoid custom icons

## Resources

- [Codicon Icon Reference](https://microsoft.github.io/vscode-codicons/dist/codicon.html)
- [VS Code Theme Color Reference](https://code.visualstudio.com/api/references/theme-color)
- [VS Code UX Guidelines](https://code.visualstudio.com/api/ux-guidelines/overview)
