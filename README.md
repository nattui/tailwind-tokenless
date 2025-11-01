# @nattui/tailwind-exact

**Precision styling, mapped one to one**

A Tailwind CSS theme library providing pixel-perfect utility classes with exact, precise spacing and sizing values. Perfect for design systems that require precise control over measurements.

## Features

- 🎯 **Precision styling** - Exact spacing and sizing values mapped one-to-one
- 📏 **Two base scales** - Available in base 10 and base 16 configurations
- 🎨 **Comprehensive utilities** - Container, spacing, text, radius, shadows, blur, and more
- ⚡ **Tailwind v4 compatible** - Built with modern `@theme` syntax
- 📦 **Lightweight** - Import only what you need

## Installation

```bash
npm install @nattui/tailwind-exact
# or
bun add @nattui/tailwind-exact
# or
yarn add @nattui/tailwind-exact
```

## Usage

### Base 10 Scale

```css
@import "@nattui/tailwind-exact";
```

### Base 16 Scale

```css
@import "@nattui/tailwind-exact/styles/16/index.css";
```

### Individual Utilities

Import specific utilities as needed:

```css
@import "@nattui/tailwind-exact/styles/10/spacing.css";
@import "@nattui/tailwind-exact/styles/10/text.css";
@import "@nattui/tailwind-exact/styles/shadow.css";
```

## Available Utilities

### Spacing
Precise spacing values from 0 to 384 (in 0.1rem increments for base 10, or equivalent for base 16).

### Text Sizes
Exact text sizing from 12px to 128px with custom intermediate sizes.

### Radius
Border radius utilities for consistent rounded corners.

### Container
Container sizing utilities for responsive layouts.

### Shadows & Effects
- Drop shadow
- Inset shadow
- Text shadow
- Blur effects
- Perspective dramatic effects

### Typography
- Font weight
- Line height (leading)
- Letter spacing (tracking)

### Layout
- Aspect ratio utilities
- Breakpoint utilities

## Examples

```html
<!-- Spacing -->
<div class="p-10 m-20">Precise padding and margin</div>

<!-- Text -->
<h1 class="text-24">Exact text size</h1>

<!-- Radius -->
<div class="rounded-12">Precise border radius</div>
```

## Version Structure

The library provides two main versions:

- **`styles/10/`** - Base 10 scale (default)
- **`styles/16/`** - Base 16 scale

Each version includes:
- `container.css` - Container utilities
- `radius.css` - Border radius utilities
- `spacing.css` - Spacing utilities
- `text.css` - Text size utilities
- `index.css` - Complete bundle with all utilities

## Development

```bash
# Format code
bun run format

# Fix formatting
bun run format:fix

# Update dependencies
bun run update
```
