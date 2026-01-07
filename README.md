# Architectural Testimonials Module

This repository contains a high-fidelity, responsive client testimonials component designed for modern architectural and design portfolios. The module features dual-directional infinite vertical scrolling, CSS isolation for seamless integration, and a sophisticated aesthetic rooted in minimalist design principles.
<img width="1920" height="1257" alt="module" src="https://github.com/user-attachments/assets/fe1035cd-fd2d-44db-b527-4cc71f6cd68a" />

## Live Preview

**[View Live Demo](https//:lefajmofokeng.github.io/Module/)**

---

## Technical Overview

The module is engineered using a **CSS-only animation logic**, eliminating the need for heavy JavaScript observers while maintaining smooth performance. It utilizes a "cloning" technique within the DOM to create a seamless loop.

### Core Architecture

* **CSS Isolation**: All styles are encapsulated using the `tz-` prefix to prevent namespace collisions when integrated into existing projects.
* **Dynamic Layout**: Built with CSS Grid and Flexbox, the component transitions from a 1.2:0.8 split-screen layout to a stacked vertical layout for mobile devices.
* **Variable-Driven Design**: Centralized theme management via `:root` CSS variables for rapid brand customization (colors, spacing, and typography).

### Animation Logic

The component employs two distinct animation paths:

1. **`tz-scroll-up`**: Translates the first column from `0` to `-50%` of its total height.
2. **`tz-scroll-down`**: Translates the second column from `-50%` to `0`.
3. **Pause on Interaction**: The `animation-play-state: paused` property is triggered on hover to allow users to read specific testimonials without interruption.

---

## Implementation & Integration

### Ideal Use Cases

This module is specifically optimized for:

* **Architecture & Interior Design Portfolios**: Highlighting high-end residential or commercial projects.
* **SaaS Landing Pages**: Showcasing social proof in a compact, high-energy format.
* **Creative Agencies**: Demonstrating attention to detail and interactive UI capabilities.

### Cross-Technology Compatibility

While built with vanilla HTML/CSS, this module is structured for easy porting into:

* **React/Next.js**: The internal structure can be mapped to a functional component where testimonial data is passed via a JSON object.
* **Webflow**: The CSS logic can be replicated using Webflow’s native Interaction API or custom code embeds.
* **WordPress**: Ideal for use as a custom Gutenberg block or within Elementor via HTML/CSS widgets.

---

## Configuration

To customize the component, modify the following variables in `styles.css`:

| Variable | Description |
| --- | --- |
| `--tz-color-accent` | Primary brand color used for the CTA and highlights. |
| `--tz-gap` | Controls the consistent gutter between all cards. |
| `--tz-border-radius-xl` | The curvature of the main component container. |
| `--tz-font-family` | Defaults to Inter Tight; can be replaced with any sans-serif stack. |

---

## License

This project is licensed under the MIT License. You are free to use, modify, and distribute this component in both personal and commercial projects.
