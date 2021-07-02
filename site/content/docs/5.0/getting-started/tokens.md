---
layout: docs
title: Tokens
description: Design tokens are the visual design atoms of the design system — specifically, they are named entities that store visual design attributes. 

group: getting-started
toc: true
---

## Design Tokens

Design tokens are all the values needed to construct and maintain a design system — spacing, color, typography, object styles, animation, etc.

<iframe style="border: 1px solid rgba(0, 0, 0, 0.1);" width="800" height="450" src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FGwcmnRFu2MmHaHfoyC7otD%2FCAD%3Fnode-id%3D386%253A1412" allowfullscreen></iframe>

## Code Tokens

We use them in place of hard-coded values (such as hex values for color or pixel values for spacing) in order to maintain a scalable and consistent visual system for UI development.

```css

:root {
    --cad-color-blue: #536ab1;
    --cad-color-red: #d7373f;
    --cad-color-orange: #da7b11;
    --cad-color-green: #268e6c;
    --cad-color-white: #fff;
    --cad-color-gray: #576172;
    --cad-color-gray-dark: #2f353e;
    --cad-color-gray-100: #d2d6dd;
    --cad-color-gray-200: #b8bec9;
    --cad-color-gray-300: #9ea6b5;
    --cad-color-gray-400: #848ea1;
    --cad-color-gray-500: #6b778c;
    --cad-color-gray-600: #576172;
    --cad-color-gray-700: #434b58;
    --cad-color-gray-800: #2f353e;
    --cad-color-gray-900: #1b1f24;
    --cad-spacer-0: 0;
    --cad-spacer-1: 0.25rem;
    --cad-spacer-2: 0.5rem;
    --cad-spacer-3: 1rem;
    --cad-spacer-4: 1.5rem;
    --cad-spacer-5: 3rem;
    --cad-fs-1: 1.5rem;
    --cad-fs-2: 1.25rem;
    --cad-fs-3: 1rem;
    --cad-fs-lg: 1.25rem;
    --cad-fs-sm: 0.875rem;
    --cad-fs-xs: 0.75rem;
    --cad-radius-none: 0;
    --cad-radius-sm: 0.25rem;
    --cad-radius-md: 0.5rem;
    --cad-radius-lg: 0.75rem;
    --cad-radius-round: 50rem;
    --cad-opacity-100: 1;
    --cad-opacity-75: 0.75;
    --cad-opacity-50: 0.5;
    --cad-opacity-25: 0.25;
    --cad-opacity-0: 0;
    --cad-font-sans-serif: "Roboto", sans-serif;
}

```