# The `<table>` Tag in HTML

Tables! You've seen them everywhere—from Excel spreadsheets to data-heavy websites. Let's explore how you can create your own using HTML. Understanding the `<table>` tag and its child elements is essential for organizing and displaying tabular data on the web.

## `<table>` tag

First things first, the `<table>` tag serves as the foundation of your table. It's the container for all the other table elements you'll learn about. Here's a skeleton example:

```html
<table>
  <!-- Table elements go here -->
</table>
```

## Sections of a Table

Your table can be divided into three main sections:

### 1. `<thead>`

This is the table header. It usually contains column names or labels. Anything you put here appears at the top of the table.

```html
<table>
  <thead>
    <tr>
      <th>Name</th>
      <th>Age</th>
      <th>Email</th>
    </tr>
  </thead>
  <!-- More sections -->
</table>
```

### 2. `<tbody>`

The bulk of your data goes here, in the table body.

```html
<table>
  <!-- ... -->
  <tbody>
    <tr>
      <td>John</td>
      <td>30</td>
      <td>john@example.com</td>
    </tr>
  </tbody>
</table>
```

### 3. `<tfoot>`

Rarely used but important for semantic reasons, the table footer often contains summary rows or notes.

```html
<table>
  <!-- ... -->
  <tfoot>
    <tr>
      <td colspan="2">Total People</td>
      <td>1</td>
    </tr>
  </tfoot>
</table>
```

## Table Row: `<tr>`

Rows are created using the `<tr>` tag. Every `<tr>` can contain multiple cells (`<td>` or `<th>`), one for each column.

```html
<tr>
  <td>Data 1</td>
  <td>Data 2</td>
</tr>
```

## Table Cell

You've got two types of cells:

### 1. `<th>`

This stands for "table header." Use it for column or row headings.

```html
<th>Column Title</th>
```

### 2. `<td>`

Short for "table data," this is where your actual content goes.

```html
<td>Your data here</td>
```

## Spanning Columns or Rows

Want a cell to span multiple columns or rows? Use the `colspan` or `rowspan` attributes.

```html
<td colspan="2">I span two columns!</td>
<td rowspan="2">I span two rows!</td>
```

## `<colgroup>` and `<col>`

You can use these tags to apply styles to entire columns without affecting the rows.

```html
<table>
  <colgroup>
    <col style="background-color: yellow;" />
    <col style="background-color: green;" />
  </colgroup>
  <!-- ... -->
</table>
```

And there you have it! You're now well-equipped to create tables in HTML. Happy coding!
