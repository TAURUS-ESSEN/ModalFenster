<a href="https://taurus-essen.github.io/ModalFenster/" target="_blank"> DEMO </a>
# Simple and Reusable Modal Window in JavaScript

This is a lightweight, flexible modal window implementation with smooth animation, blurred background, and support for multiple trigger buttons.

## 🚀 Features

- Smooth show/hide animation
- Background blur effect on open
- Modal closes on:
  - Close button (×)
  - Clicking outside the modal form
  - Pressing the `Escape` key
- Supports multiple modals via `data-window-id`
- Prevents duplicate event listeners

## 🧠 How It Works

Each open button has a `data-window-id` attribute that matches a modal with the same `data-window-id`.  
The modal is selected dynamically and opened with a single reusable logic.

Event listeners are attached only once per modal using a `data-listener-attached` flag.

## 📁 Files

- `index.html` — Markup with trigger buttons and modal windows
- `style.css` — Styling and transitions
- `main.js` — JavaScript logic for opening, closing, and interaction

## ✅ Usage

Add a trigger button like this:

```html
<button data-window-id="1">Open Modal</button>
