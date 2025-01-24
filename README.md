# Tailwind Tokenless

Tailwind CSS without tokens.

## Getting started

### Installation

```zsh
npm install @nattui/tailwind-tokenless
```

### Usage

`styles/global.css`

```css
@import "tailwindcss";
@import "@nattui/tailwind-tokenless";

html {
  font-size: 10px;
}
```

or

```css
/* Order matters */
@import "tailwindcss";
@import "@nattui/tailwind-tokenless/styles/index.css";
@import "@nattui/tailwind-tokenless/styles/colors/reset.css";
@import "@nattui/tailwind-tokenless/styles/colors/gray/mauve.css";
@import "@nattui/tailwind-tokenless/styles/colors/gray/mauve-alpha.css";
@import "@nattui/tailwind-tokenless/styles/colors/crimson.css";

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
