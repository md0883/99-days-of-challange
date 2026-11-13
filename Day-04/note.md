#Day 04 — HTML Tables & Forms

1. HTML Tables

HTML tables help us display information in an organized way using rows and columns. They are useful when we need to show things like student information, marks, schedules or other structured data.

> Common Table Tags

| Tag | What it does |
|---|---|
| `<table>` | Creates a table |
| `<thead>` | Contains the heading section |
| `<tbody>` | Contains the main table data |
| `<tfoot>` | Contains the footer section |
| `<tr>` | Creates a new row |
| `<th>` | Defines a heading cell |
| `<td>` | Adds data to a cell |
| `<caption>` | Gives the table a title |

>Basic Table Example

```html
<table border="1">
    <thead>
        <tr>
            <th>Name</th>
            <th>Department</th>
            <th>Semester</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>Rahim</td>
            <td>CSE</td>
            <td>5th</td>
        </tr>

        <tr>
            <td>Karim</td>
            <td>SWE</td>
            <td>6th</td>
        </tr>
    </tbody>
</table>
```

>A Few Useful Table Attributes

- `colspan` — Used when one cell needs to cover multiple columns.
- `rowspan` — Used when one cell needs to cover multiple rows.
- `border` — Adds a border to a table. This is an older HTML attribute; CSS is normally used for styling borders.

2. HTML Forms

HTML forms are used to collect information from users. For example, when someone creates an account, fills out a registration form or logs into a website, they are interacting with HTML forms.

>Basic Form Structure

```html
<form action="/register" method="post">

    <label for="name">Full Name:</label>
    <input type="text" id="name" name="name">

    <button type="submit">Submit</button>

</form>
```
>Important Form Attributes

| Attribute | What it does |
|---|---|
| `action` | Defines where the form data will be sent |
| `method` | Defines how the data will be submitted |
| `name` | Identifies a field when form data is submitted |
| `required` | Makes a field compulsory |
| `autocomplete` | Controls whether the browser suggests previously entered information |
| `novalidate` | Turns off the browser's built-in form validation |
| `enctype` | Defines how the form data is encoded when submitted |

>Difference Between GET and POST

>GET Method

- Sends form information through the URL.
- Useful for search forms and filtering data.
- Submitted information can appear in browser history.

>POST Method

- Sends form information in the request body.
- Commonly used for registration and login forms.
- Does not automatically encrypt information, so HTTPS is still important.

3. HTML Input Types

The `<input>` element is one of the most important parts of an HTML form. It allows users to enter different types of information depending on the input type we choose.

### Common Input Types

| Input Type | Purpose |
|---|---|
| `text` | Enter normal text |
| `password` | Enter a password |
| `email` | Enter an email address |
| `number` | Enter numeric values |
| `tel` | Enter a phone number |
| `url` | Enter a website address |
| `date` | Select a date |
| `time` | Select a time |
| `datetime-local` | Select a date and time |
| `radio` | Choose one option from a group |
| `checkbox` | Select one or multiple options |
| `file` | Upload a file |
| `color` | Choose a color |
| `range` | Select a value using a slider |
| `search` | Enter search keywords |
| `hidden` | Store a value that is not displayed |
| `submit` | Submit the form |
| `reset` | Reset the form |
| `button` | Create a regular button |
| `month` | Select a month |
| `week` | Select a week |

>Input Examples

```html
<input type="text" placeholder="Enter your name">

<input type="email" placeholder="Enter your email">

<input type="password" placeholder="Enter your password">

<input type="number" min="1" max="100">

<input type="date">

<input type="radio" name="gender" value="Male">

<input type="checkbox" name="skills" value="HTML">

<input type="file">

<input type="submit" value="Submit">
```
4. HTML Labels

The `<label>` tag gives a name or description to an input field. It makes forms easier to understand and improves accessibility.

> Example

```html
<label for="email">Email Address:</label>
<input type="email" id="email" name="email">
```

>Things to Remember

- The `for` attribute connects a label to an input.
- The value of `for` must match the input's `id`.
- Clicking on a label can focus or activate its related input.
- Labels should be used for form fields so users can easily understand what information is required.

5. HTML Buttons

Buttons allow users to perform actions in a form. HTML provides different button types depending on what we want them to do.

>Three Common Button Types

1. Submit Button

```html
<button type="submit">Register</button>
```

Used to submit the form data.

2. Reset Button

```html
<button type="reset">Reset</button>
```

Returns form fields to their original values.

3. Regular Button

```html
<button type="button">Click Me</button>
```

Creates a normal clickable button. It does not submit the form automatically.

>6. Other Useful Form Elements

Apart from input fields, HTML provides some additional elements that make forms more organized and user-friendly.

### Select and Option

These tags are used to create a dropdown menu where users can choose an option.

```html
<label for="department">Department:</label>

<select id="department" name="department">
    <option value="">Select Department</option>
    <option value="CSE">CSE</option>
    <option value="SWE">SWE</option>
    <option value="EEE">EEE</option>
</select>
```

>Textarea

The `<textarea>` element allows users to write longer messages or descriptions instead of entering everything on a single line.

```html
<label for="message">Message:</label>

<textarea id="message" name="message" rows="5" cols="30"></textarea>
```

>Fieldset and Legend

These elements help group related form fields together. For example, we can keep all personal information inside one section and academic information inside another.

```html
<fieldset>
    <legend>Personal Information</legend>

    <label for="name">Name:</label>
    <input type="text" id="name" name="name">

</fieldset>
```

---
7. Important HTML Form Attributes

Here are some additional attributes that help control how form elements work.

| Attribute | Purpose |
|---|---|
| `placeholder` | Shows a short hint inside an input |
| `required` | Makes the field mandatory |
| `value` | Sets the initial value |
| `readonly` | Allows users to view but not edit a field |
| `disabled` | Makes a field inactive |
| `min` | Sets the minimum allowed value |
| `max` | Sets the maximum allowed value |
| `minlength` | Sets the minimum number of characters |
| `maxlength` | Sets the maximum number of characters |
| `pattern` | Sets a pattern for input validation |
| `checked` | Selects a checkbox or radio button by default |
| `selected` | Selects an option by default |
| `multiple` | Allows multiple selections |
| `accept` | Specifies which file types can be selected |

8. What I Learned Today

After practicing these topics, I now understand how different HTML elements work together to build a functional form.

Some important things I learned:

- Tables help display information in rows and columns.
- Forms are used to collect information from users.
- Different input types are available for different kinds of data.
- Labels make form fields easier to understand and use.
- The `name` attribute identifies submitted form data.
- The `id` attribute identifies an HTML element.
- Radio buttons with the same `name` allow users to select one option.
- Checkboxes allow users to select multiple options.
- The `required` attribute helps prevent users from submitting empty required fields.
- `fieldset` and `legend` help organize related form elements.
- HTML can create the structure and basic validation of a form, but saving information requires a backend or another form-processing service.


