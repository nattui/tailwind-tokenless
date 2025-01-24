# Tailwind Tokenless

Tailwind CSS without tokens.

## Getting started

### Installation

```zsh
npm install @nattui/tailwind-tokenless
```

### Usage

#### Base 16

`styles/global.css`

```css
@import "tailwindcss";
@import "@nattui/tailwind-tokenless";
```

#### Base 10

`styles/global.css`

```css
@import "tailwindcss";
@import "@nattui/tailwind-tokenless/styles/10/index.css";

html {
  font-size: 10px;
}
```

`.vscode/settings.json`

```json
{
  "tailwindCSS.rootFontSize": 10
}
```

#### Colors

`styles/global.css`

```css
/* Order matters */
@import "tailwindcss";
@import "@nattui/tailwind-tokenless/styles/colors/reset.css";
@import "@nattui/tailwind-tokenless/styles/colors/gray/mauve.css";
@import "@nattui/tailwind-tokenless/styles/colors/gray/mauve-alpha.css";
@import "@nattui/tailwind-tokenless/styles/colors/crimson.css";
```
