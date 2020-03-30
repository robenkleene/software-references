# Excel

## Keyboard Shortcuts

- `⇧␣`: Select row
- `⌃␣`: Select column
- `⇧⌃+`: Insert row (first select the row to avoid the Insert Cells dialog)
- `⇧⌃+`: Insert column (same shortcut as above?)
- `⌃U`: Edit current cell, when editing a cell, hit `⌘A` to switch to the formula bar (another option to edit in the formula bar is to turn off the "Edit Directly in Cell" preference, although this means you can never edit in the cell, even when not editing a formula)

## Navigation

- `^PgDn` / `^PgUp`: Go to next / previous worksheet

### Editing

- `⌃;`: Insert today's date
- `⇧⌃$`: Format cell as currency
- `⇧⌃%`: Format cell as percentage
- `⌃-`: Delete rows or columns
- `⌘K`: Edit shortcut
- `⌘A`: Jump between editing in the cell and in the formula bar
- `⌃A`: Select all in the formula bar

### Selection

When a group of cells are selected.

- `⌃D`: Fill down
- `⌃⌘V`: Paste special, e.g., to add or multiply all cells by the value on the clipboard

### Editing

Editing a cell when there's a selection.

- `⌃↩`: Fill all selected cells with the same value
- `⇥`: Edit the next selected cell.
- To insert a link, enter the link text, finish editing the cell, and choose "Insert > Link"

## Tips

- To clear formatting, use "Edit" -> "Clear" -> "Formats"
- A more precise way to clear formatting is to open cell styles `⌘1` and select "Font" -> "Normal Font"
- Use "Paste" -> "Paste Values" to paste the results of a formula, rather than the formula itself.
- You can give a cell or a column a variable name (use "Formulas" -> "Define Name"), and then refer to it by name in formula.

## Columns

### Re-Ordering Columns

1. First select the entire column `^␣` twice.
2. Hover over the column's border until a hand icon appears.
3. Drag the column to it's new location, a green line should be display between columns showing where the column will be moved to. (If instead an entire destination column is being highlighted, or a single cell, then a move will not happen, you probably have to select the whole column.)

## Cell Styles

Excel has some useful built-in styles under "Home" -> "Cell Styles".

- Normal
- Good
- Bad
- Neutral
- Input: Something meant to be changed
- Calculation: Something that is output

## Delimited Data

To add comma- or tab-delimited data, paste it into one cell, then select "Data" -> "Text to Columns"

1. Paste the data into one cell

## Fill Handle

Use the fill handle (little box to the bottom right of a selection box), to fill a bunch of cells with a pattern.

### Supported Lists

- Days of the week
- Dates
- Incremented or decremented numbers

## R1C1

R1C1 is Excel's "native" way of referencing cells. It can be helpful to switch to R1C1 mode (in "Preferences" -> "General" -> "Use R1C1 reference style" to see what's going on under the hood.

## Formula

- Use `⌘T` when editing a formula to switch between relative

### Symbols

- `&`: Concatenates
- `$`: Means absolute reference (as opposed to relative)
- `'`: Start the value of a cell with an apostrophe to make it plain text (e.g., to enter a number that starts with leading zeros)

