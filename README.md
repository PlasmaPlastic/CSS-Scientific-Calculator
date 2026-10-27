# Pure CSS Scientific Calculator

<p align="center">
  <img
    src="https://i.pinimg.com/736x/28/94/54/2894542729905c84629d001a68278043.jpg"
    width="300"
  >
  <img
    src="https://i.pinimg.com/736x/d1/ec/fa/d1ecfae837107adc11ca692e66ba122d.jpg"
    width="300"
  >
</p>

A functional scientific calculator built using **only CSS and HTML5**. It performs mathematical calculations without any JavaScript.

## Overview

This project implements a scientific calculator UI and calculation engine entirely within CSS by leveraging modern CSS features such as trigonometric functions, CSS variables, `:has()` relational pseudo-classes, and CSS counters.

## Features

* **No JavaScript**: All state management, calculations, and UI updates run strictly through CSS.
* **Math Operations**: Supports basic operations (`+`, `-`, `*`, `/`), trigonometric functions (`sin`, `cos`, `tan`, `asin`, `acos`, `atan`), powers (`x²`, `xʸ`), square roots (`√`), logarithms (`log`, `ln`), and angle unit toggling (`DEG` / `RAD`).
* **CSS Counters**: Displays numeric values on screen using CSS `counter-reset` and `counter()` content replacement.

## How It Works

1. **State Selection**: Form inputs (`input[type="radio"]` and `input[type="checkbox"]`) capture user selections.
2. **State Detection**: The parent container evaluates selected controls using `:has(:checked)` to assign corresponding values to CSS custom properties.
3. **Calculation**: Mathematical expressions are evaluated dynamically using nested `calc()` functions along with CSS trig and log functions.
4. **Result Rendering**: Values are separated into integer and fractional components, which are rendered visually via CSS counter properties.

## Browser Compatibility

Requires modern browsers supporting CSS Values and Units Module Level 4 (specifically `sin()`, `cos()`, `round()`, and `mod()`):

* **Chrome**: 125 or newer
* **Edge**: 125 or newer
* **Safari**: 17.4 or newer
* **Firefox**: 128 or newer
