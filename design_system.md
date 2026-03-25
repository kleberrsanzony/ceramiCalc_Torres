# Torres Modern Dark UI - Design System

This document outlines the visual style developed for the CerâmiCalc Torres project. Use these tokens and patterns to ensure consistency in future "Premium Dark" applications.

## Color Palette

| Name | Hex | Usage |
| :--- | :--- | :--- |
| **Deep Space** | `#0a0a0c` | Main application background |
| **Dark Slate** | `#121214` | Primary card background |
| **Input Base** | `#1c1c1e` | Input fields and subtle backgrounds |
| **Golden Amber** | `#facc15` | Accent color, icons, and primary highlights |
| **Vivid Purple** | `#a855f7` | Secondary accent color for specific modules |
| **Text Primary**| `#ffffff` | Headings and critical information |
| **Text Secondary**| `#94a3b8` | Supporting text and labels |
| **Border Dark** | `#27272a` | Default component borders |

## Typography

- **Font Family**: [Inter](https://fonts.google.com/specimen/Inter) (fallback: sans-serif)
- **Scale**:
    - **H1 (Hero)**: `2.5rem`, Weight: `800`, Background clip: `text`, Gradient: `linear-gradient(135deg, #fff 0%, #a1a1aa 100%)`.
    - **H2 (Section)**: `1.25rem` to `1.5rem`, Weight: `700`.
    - **Labels**: `0.9rem`, Weight: `500`, Color: `text-secondary`.
    - **Result Values**: `2.2rem` to `3rem`, Weight: `800`, Color: `accent-color`.

## UI Components

### Premium Cards
- **Radius**: `20px` (large) or `16px` (medium).
- **Border**: `1px solid #27272a`.
- **Shadow**: Deep, soft shadows (`box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.5)`).
- **Glowing Indicator**: A `2px` top border with a linear gradient and low opacity.
- **Hover States**: Subtle vertical movement (`translateY(-5px)`) and increased border contrast.

### Layout Patterns
- **Responsive Symmetry**: 2-column grid on desktop that stacks on mobile.
- **Micro-animations**: Use `transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1)` for all interactions.

## CSS Implementation

```css
:root {
    --bg-color: #0a0a0c;
    --card-bg: #121214;
    --input-bg: #1c1c1e;
    --accent-color: #facc15; /* Golden Amber */
    --secondary-accent: #a855f7; /* Vivid Purple */
    --text-primary: #ffffff;
    --text-secondary: #94a3b8;
    --border-color: #27272a;
    --card-radius: 20px;
    --transition: all 0.3s cubic-bezier(0.4, 0, 0.2, 1);
}
```
