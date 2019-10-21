# Microsoft Excel

## Keyboard Shortcuts

- `⇧␣`: Select row
- `⇧⌃+`: Insert row (first select the row to avoid the Insert Cells dialog)
- `⌃U`: Edit current cell, when editing a cell, hit `⌘A` to switch to the formula bar (another option to edit in the formula bar is to turn off the "Edit Directly in Cell" preference, although this means you can never edit in the cell, even when not editing a formula)

### Editing

- `⌃;`: Insert today's date
- `⇧⌃$`: Format cell as currency
- `⇧⌃%`: Format cell as percentage
- `⌃-`: Delete rows

### Selection

When a group of cells are selected.

- `⌃D`: Fill down
- `⌃⌘V`: Paste special, e.g., to add or multiply all cells by the value on the clipboard

#### Editing

Editing a cell when there's a selection.

- `⌃↩`: Fill all selected cells with the same value
- `⇥`: Edit the next selected cell.

## Tips

- Use "Paste" -> "Paste Values" to paste the results of a formula, rather than the formula itself.
- You can give a cell or a column a variable name (use "Formulas" -> "Define Name"), and then refer to it by name in formula.
- To re-order columns: Select the column you want to move, then hover over its border and hold shift while dragging to move it into a new location (if you don't hold shift, it will replace the destination column).

## Cell Styles

Excel has some useful built-in styles under "Home" -> "Cell Styles".

- Normal
- Good
- Bad
- Neutral
- Input: Something meant to be changed
- Calculation: Something that is output

## Tables

- Select a range and "Home" -> "Format as Table"
- With any cell in the table selected, "Table" -> "Total Row"

### Keyboard Shortcuts

- `⇥`: Create a new row when the last cell in the table is selected

## Fill Handle

Use the fill handle (little box to the bottom right of a selection box), to fill a bunch of cells with a pattern.

### Supported Lists

- Days of the week
- Dates
- Incremented or decremented numbers

## R1C1

R1C1 is Excel's "native" way of referencing cells. It can be helpful to switch to R1C1 mode (in "Preferences" -> "General" -> "Use R1C1 reference style" to see what's going on under the hood.

## Formula

- Use `⌘T` when editing a formula to switch between a relative 

### Symbols

- `&`: Concatenates
- `$`: Means absolute reference (as opposed to relative)
- `'`: Start the value of a cell with an apostrophe to make it plain text (e.g., to enter a number that starts with leading zeros)

