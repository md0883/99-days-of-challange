# Day 09 Notes — CSS Grid, Positioning & Selectors

Today I worked on three useful parts of CSS: arranging content with Grid, controlling where elements appear, and selecting elements in more specific ways.

## 1. CSS Grid

CSS Grid is a layout system that helps arrange elements in rows and columns. It is useful when a page needs a structured layout, such as an image gallery.

>Important properties

| Property | What it does |
|---|---|
| `display: grid` | Turns an element into a grid container |
| `grid-template-columns` | Sets the column structure |
| `grid-template-rows` | Sets the row structure |
| `gap` | Adds space between grid items |
| `grid-column` | Controls which columns an item occupies |
| `grid-row` | Controls which rows an item occupies |

>Example

```css
.gallery {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
}
```

`fr` means a fraction of the available space. In this example, the three columns share the available width equally.

>A flexible grid

```css
.gallery {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
    gap: 24px;
}
```

- `minmax(280px, 1fr)` gives each column a minimum width of 280px and lets it grow.
- `auto-fit` fits as many columns as the available space allows.

## 2. CSS Positioning

The `position` property controls how an element is placed on a page.

| Value | Meaning |
|---|---|
| `static` | Default position in the normal document flow |
| `relative` | Keeps its normal place but can be shifted |
| `absolute` | Positioned relative to its nearest positioned ancestor |
| `fixed` | Positioned relative to the browser window |
| `sticky` | Acts normally until it reaches a defined scroll position |

The `top`, `right`, `bottom` and `left` properties can be used to adjust positioned elements.

>Example

```css
.image-wrap {
    position: relative;
}

.image-number {
    position: absolute;
    top: 16px;
    left: 16px;
}
```

Here, the image number is placed inside the image wrapper. The wrapper uses `relative`, while the number uses `absolute`.

## 3. Pseudo-classes

A pseudo-class selects an element based on its state or position.

| Selector | Use |
|---|---|
| `:hover` | When the pointer is over an element |
| `:focus` | When an element receives focus |
| `:first-child` | Selects the first child |
| `:last-child` | Selects the last child |
| `:nth-child()` | Selects a child by its position |

>Example

```css
.gallery-card:hover img {
    transform: scale(1.04);
}
```

This slightly enlarges the image when the user hovers over its card.

## 4. Pseudo-elements

Pseudo-elements let us style a specific part of an element or add decorative content.

| Selector | Use |
|---|---|
| `::before` | Adds generated content before an element's content |
| `::after` | Adds generated content after an element's content |
| `::first-letter` | Styles the first letter |
| `::first-line` | Styles the first line |

>Example

```css
.image-wrap::after {
    content: "";
    position: absolute;
    inset: 45% 0 0;
    background: linear-gradient(transparent, rgba(0, 0, 0, .5));
}
```

This creates a dark gradient over the lower part of an image. The `content` property is needed for the pseudo-element to appear.

## 5. What I used in Pixel Stories

- CSS Grid arranges the six photo cards.
- `auto-fit` and `minmax()` allow the columns to adapt to the available width.
- `position: relative` creates a positioning reference for each image card.
- `position: absolute` places the image number and category label.
- `:hover` adds a small image zoom effect.
- `::after` creates the gradient overlay.
