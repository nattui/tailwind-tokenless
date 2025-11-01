# Tailwind Tokenless

Tailwind CSS without tokens

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
@import "@nattui/tailwind-tokenless/styles/16/index.css";
```

#### Base 10

`styles/global.css`

```css
@import "tailwindcss";
@import "@nattui/tailwind-tokenless";

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
