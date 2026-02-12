# Flexbox Decisions

This document explains the Flexbox layout choices used throughout the project and why they were appropriate for each layout.

---

## Dashboard Layout

Flexbox was used to structure the dashboard because the layout required flexible spacing between navigation, main content, and widgets. A row-based Flexbox container allowed sections to align side-by-side on larger screens while still wrapping naturally on smaller screens. Flex properties such as `flex-grow` and `flex-basis` were used to control the relative size of each panel without relying on fixed widths.

---

## Product Page Layout

Flexbox was chosen for the product page to support a responsive, real-world e-commerce layout. The product gallery and information panel were placed inside a Flexbox container with wrapping enabled so they appear side-by-side on wide screens and stack on narrow screens. The image thumbnail strip uses Flexbox with a gap to evenly space thumbnails.

The specifications section uses Flexbox with wrapping and a flexible basis to create responsive columns that adapt to available space. Reviews were built using the media object pattern, where avatars have fixed sizing and content expands to fill the remaining space.

---

## Article Layout

Flexbox was used in the article hero section to vertically center content and push metadata to the bottom using `margin-top: auto`. This approach allows the hero to adapt to different text lengths while maintaining visual balance.

The main article and sidebar use proportional Flexbox sizing to create a magazine-style layout that remains responsive. Pull quotes use `align-self` to break out of the normal text flow and create visual emphasis. Related articles and the author bio follow the media object pattern, ensuring consistent alignment between images and text.

---

## Why Flexbox Was Used

Flexbox was chosen throughout the project because it provides flexible alignment, spacing, and ordering of elements without relying on fixed positioning or excessive media queries. This makes the layouts more maintainable and responsive across different screen sizes.
