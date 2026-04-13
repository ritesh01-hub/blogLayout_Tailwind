# Responsive Blog Layout in Tailwind CSS

A clean and responsive blog layout built with pure HTML, Tailwind CSS, and vanilla JavaScript. Features a collapsible sidebar, blog post cards, and a modal popup for reading post previews.

---

## Features

- **Collapsible Sidebar** — Slide-in panel with author profile and popular posts list
- **Blog Post Grid** — Responsive 1/2/3-column grid of post cards with images and descriptions
- **Modal Popup** — Clicking "Read More" opens a modal with the post's image and full content
- **Smooth Animations** — CSS transitions on sidebar toggle, card hover lift, and list hover slide
- **Fully Responsive** — Mobile-first layout using Tailwind's responsive breakpoints

---

## Tech Stack

| Technology | Version |
|---|---|
| HTML5 | — |
| Tailwind CSS | 2.2.19 (CDN) |
| JavaScript | Vanilla (ES6) |

---

## Getting Started

No build tools or installation needed. Just open the file directly in your browser.

```bash
# Option 1 — Open directly
Double-click Blog_Layout_in_Tailwind_CSS.html

# Option 2 — VS Code Live Server
Right-click the file → Open with Live Server
```

---

## Project Structure

```
Blog_Layout_in_Tailwind_CSS.html    # All-in-one file (HTML + Tailwind + JS)
```

---

## How It Works

### Sidebar
- Hidden off-screen by default via `-translate-x-full`
- Toggled open/close by clicking the hamburger icon (top-left)
- Displays author name (Ritesh Tiwari), bio, and 6 popular post links with thumbnails

### Blog Post Grid
- Renders 6 post cards in a responsive CSS grid (`1 col → 2 col → 3 col`)
- Each card has a cover image, title, short description, date, and a "Read More" link
- Cards lift on hover via `hover:-translate-y-1`

### Modal
- Triggered by any `.read-more` link (both sidebar and grid cards)
- Post content is injected dynamically using the `data-title` attribute
- Closed via the "Close" button which re-adds the `hidden` class

---

## Blog Posts

| Title | Date |
|---|---|
| Responsive Web Design | March 21, 2024 |
| JavaScript Fundamentals | March 18, 2024 |
| CSS Flexbox Tutorial | March 15, 2024 |
| HTML Basics | March 10, 2024 |
| CSS Grid Layout | March 5, 2024 |
| React Hooks | February 28, 2024 |

---

## Customization

**Change author info** — Edit the name, role, and bio text inside the sidebar `<div>`

**Add a new post card** — Copy any `.blog-post` div in the grid, update the image `src`, title, description, and `data-title`

**Add modal content** — In the `<script>` block, add a new `else if` matching the new post's `data-title`

**Replace images** — Swap out any `src` URL in the `<img>` tags with your own hosted images

---

