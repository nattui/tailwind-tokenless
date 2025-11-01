# Pixelwind

> Precision styling for developers who think in pixels

Pixelwind is a Tailwind CSS v4 theme that replaces abstract design tokens with intuitive pixel-based values. Say goodbye to memorizing what `spacing-4` means—with Pixelwind, the class names match the actual pixel dimensions.

## Why Pixelwind?

Traditional design systems use arbitrary tokens (`spacing-4`, `spacing-8`) that require mental translation. Pixelwind eliminates this cognitive overhead:

- **Intuitive**: `spacing-24` means 24 pixels
- **Predictable**: Class names directly correspond to pixel values
- **Flexible**: Choose between 10px or 16px base font sizes
- **Modern**: Built for Tailwind CSS v4's `@theme` directive

## Installation

```bash
npm install @nattui/pixelwind
# or
pnpm add @nattui/pixelwind
# or
bun add @nattui/pixelwind
```

## Usage

Import Pixelwind in your CSS file:

```css
/* For 10px base (1rem = 10px) */
@import "@nattui/pixelwind";

/* OR for 16px base (1rem = 16px) */
@import "@nattui/pixelwind/styles/16/index.css";
```

Then use the classes in your HTML:

```html
<div class="p-24 m-16 shadow-4 rounded-8">
  <!-- padding: 24px, margin: 16px -->
</div>
```

## Base Size Variants

### 10px Base (`styles/10/`)

- `spacing-10` = 1rem = 10px
- `spacing-20` = 2rem = 20px
- Ideal for designs that prefer decimal simplicity

### 16px Base (`styles/16/`)

- `spacing-16` = 1rem = 16px
- `spacing-32` = 2rem = 32px
- Aligns with browser defaults and accessibility standards

## Available Utilities

Pixelwind includes pixel-perfect values for:

- **Spacing**: `0`, `1`, `2`, `4`, `6`, `8`, `10`, `12`, `14`, `16`, `20`, `24`, `28`, `32`, `36`, `40`, `44`, `48`, `56`, `64`, `80`, `96`, `112`, `128`, `144`, `160`, `176`, `192`, `208`, `224`, `240`, `256`, `288`, `320`, `384`
- **Shadows**: `shadow-0` through `shadow-7`
- **Text Shadows**: Custom text shadow utilities
- **Drop Shadows**: Filter-based drop shadows
- **Inset Shadows**: Inner shadow effects
- **Blur**: Backdrop and regular blur values
- **Border Radius**: Consistent rounded corner values
- **Typography**: Font weights, line heights, letter spacing
- **Containers**: Max-width container utilities
- **Aspect Ratios**: Common aspect ratio utilities
- **Breakpoints**: Responsive design breakpoints
- **Perspective**: 3D transform perspective values

## Importing Individual Utilities

You can also import specific utilities instead of the entire bundle:

```css
@import "@nattui/pixelwind/styles/10/spacing.css";
@import "@nattui/pixelwind/styles/shadow.css";
@import "@nattui/pixelwind/styles/blur.css";
```

## Tailwind CSS v4 Compatibility

Pixelwind is built for Tailwind CSS v4 and uses the modern `@theme` directive to define CSS custom properties. Make sure you're using Tailwind CSS v4 or later.

## Philosophy

Design systems often abstract values to maintain consistency, but this comes at a cost: cognitive overhead. When a developer sees `spacing-4`, they need to remember or look up what that means in pixels.

Pixelwind takes a different approach: **the class name IS the value**. This eliminates translation overhead while maintaining the power and flexibility of Tailwind's utility-first approach.
