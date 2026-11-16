# Day 07 — CSS Box Model, Margin, Padding, Border & Display

1. CSS Box Model

Every HTML element displayed on a webpage is treated as a rectangular box by CSS. This structure is known as the **CSS Box Model**.

The box model explains how the content, padding, border, and margin work together to determine the space an element occupies.

>Four Parts of the Box Model

1. Content:The actual text, image, or other content inside an element.
2. Padding: The space between the content and the border.
3. Border: The line surrounding the content and padding.
4. Margin: The space outside the border that separates an element from others.

>Box Model Structure

```text
        MARGIN
  ┌───────────────────────┐
  │        BORDER         │
  │  ┌─────────────────┐  │
  │  │     PADDING     │  │
  │  │  ┌───────────┐  │  │
  │  │  │  CONTENT  │  │  │
  │  │  └───────────┘  │  │
  │  └─────────────────┘  │
  └───────────────────────┘
```

>Example

```css
.card {
    width: 250px;
    padding: 20px;
    border: 2px solid #333;
    margin: 15px;
}
```
In this example:

- Content width = 250px
- Left and right padding = 40px
- Left and right border = 4px
- Left and right margin = 30px

Total horizontal space occupied = 324px.
The calculation is:

`250 + 40 + 4 + 30 = 324px`

This is the default `content-box` calculation.

2. CSS Margin

Margin creates space outside an element's border. It helps separate one element from another.
>Margin Properties

```css
.card {
    margin: 20px;
}
```
This applies 20px of margin to all four sides.
We can also control each side separately:

```css
.card {
    margin-top: 10px;
    margin-right: 20px;
    margin-bottom: 15px;
    margin-left: 20px;
}
```
>Margin Shorthand
CSS allows us to write margin values in a shorter way.

```css
.card {
    margin: 10px 20px 15px 20px;
}
```

The order is:

`top → right → bottom → left`

Other useful examples:

```css
margin: 20px;
margin: 10px 20px;
margin: 10px 15px 20px;
```
- One value: All four sides.
- Two values: Top and bottom, then left and right.
- Three values: Top, left and right, then bottom.
- Four values: Top, right, bottom, and left.

>3. CSS Padding

Padding creates space inside an element, between its content and border.
It helps prevent text or other content from touching the border.

>Example

```css
.card {
    padding: 20px;
}
```
This creates 20px of internal space on all four sides.
>Individual Padding Properties

```css
.card {
    padding-top: 15px;
    padding-right: 20px;
    padding-bottom: 15px;
    padding-left: 20px;
}
```
>Padding Shorthand

```css
.card {
    padding: 15px 20px;
}
```
This applies 15px to the top and bottom and 20px to the left and right.
>Remember: Margin controls outside spacing, while padding controls inside spacing.

## 4. CSS Border

A border creates a visible boundary around an HTML element. It appears outside the padding and around the content area.
>Basic Border Syntax

```css
.card {
    border: 2px solid #333;
}
```
The three main parts are:
- Width: `2px`
- Style: `solid`
- Color: `#333`

>Common Border Styles

```css
border: 2px solid black;
border: 2px dashed black;
border: 2px dotted black;
border: 2px double black;
```

>Individual Border Properties

```css
.card {
    border-width: 2px;
    border-style: solid;
    border-color: #333;
}
```

We can also style individual sides:

```css
.card {
    border-top: 2px solid black;
    border-right: 2px dashed black;
    border-bottom: 2px solid black;
    border-left: 2px dotted black;
}
```

5. CSS Display Property

The `display` property determines how an HTML element behaves in the document layout.

Different display values affect whether elements start on a new line, sit beside other elements, or are hidden.

>A. Display: Block

A block element starts on a new line and normally takes up the available width of its parent.
Examples include:

- `div`
- `p`
- `h1`
- `section`

```css
.card {
    display: block;
}
```

>B. Display: Inline

An inline element stays within the same line as surrounding content. It only takes up the space its content needs.
Examples include:

- `span`
- `a`
- `strong`

```css
.label {
    display: inline;
}
```
Width and height do not work on inline elements in the same way they do on block or inline-block elements.

>C. Display: Inline-block

An inline-block element can sit beside other elements like an inline element, but it also allows us to set its width and height like a block element.

```css
.card {
    display: inline-block;
    width: 250px;
}
```

This is useful for creating simple card layouts without Flexbox or Grid.

 >D. Display: None

The `display: none` value completely removes an element from the layout. It does not occupy any space on the page.

```css
.hidden {
    display: none;
}
```

The element is not displayed until its display value is changed.

6. Practical Application — The CSS Learning Corner

For today's practical task, I created a three-card layout using HTML and CSS.

The project demonstrates:

- The relationship between content, padding, border, and margin.
- How spacing changes the appearance of individual cards.
- How `inline-block` places cards beside each other.
- How `block`, `inline`, and `none` can be used for different element behaviors.

7. Quick Revision

| Property | Main Purpose |
|---|---|
| Content | Holds the actual element content |
| Padding | Creates space inside the border |
| Border | Surrounds the content and padding |
| Margin | Creates space outside the border |
| `display: block` | Starts on a new line |
| `display: inline` | Stays within the text flow |
| `display: inline-block` | Sits inline while supporting dimensions |
| `display: none` | Removes the element from the layout |
